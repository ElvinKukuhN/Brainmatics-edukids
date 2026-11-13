# Self-hosted PostgreSQL on a VPS, with access rules enforced by row-level security

EduKids LMS runs as Next.js (TypeScript) and PostgreSQL together on one VPS under Docker Compose. Database access goes through Drizzle, and Better Auth handles email-and-password login, storing users in the same PostgreSQL. We deliberately chose plain PostgreSQL over Supabase or a managed database so we keep full control of the server and the data, at the cost of running backups and operations ourselves.

Access rules are enforced by PostgreSQL row-level security, not only in application code: Tutors write only to their own Classes, Parents read only their own children, and only Admins change master data. The app sets the current user's identity on every transaction, and the policies read it. The Software Request requires that no unauthorised access is possible, and putting the rules in the database means a missed check in the app can't leak one family's data to another.

The Software Request also requires a backup every 24 hours, stored somewhere other than the system. A scheduled `pg_dump` runs daily and copies the dump off the VPS to separate storage.
