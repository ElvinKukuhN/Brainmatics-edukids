# EduKids LMS

A learning management system for a primary-school (SD) tutoring centre running Mathematics and English programs. It tracks attendance per Session, scores per Competency Aspect, and each Student's Level progression in every Subject.

Each term lists its Indonesian label, which is the word used on screen.

## Language

### People

**Admin**:
A staff member who owns master data, places Students into Classes, runs Levelling and publishes Report Cards.
_Label_: Admin Akademik
_Avoid_: Administrator, Operator

**Tutor**:
A staff member who teaches Classes and records Attendance, Scores and Tutor Notes for them.
_Label_: Pengajar
_Avoid_: Teacher, Guru

**Parent**:
A person who follows the progress of one or more Students (their children) and can only view, never change, their data.
_Label_: Orang Tua
_Avoid_: Guardian, Wali

**Student**:
A primary-school child taking one or more Subjects at the centre. A Student does not log in.
_Label_: Siswa
_Avoid_: Murid, Pupil, Learner

### Curriculum

**Subject**:
A program of study offered by the centre, such as Mathematics or English.
_Label_: Mata Pelajaran
_Avoid_: Program, Course, Mapel (in writing)

**Level**:
One step in a Subject's ordered sequence of difficulty. A Student holds exactly one Level in each Subject they take.
_Label_: Level
_Avoid_: Grade, Stage, Tingkat

**Competency Aspect**:
A specific skill within a Subject on which Students are scored, such as Listening in English.
_Label_: Aspek Kompetensi
_Avoid_: Component, Skill, Indicator

### Enrollment and classes

**Enrollment**:
The fact that a Student takes a particular Subject.
_Label_: Pendaftaran Mata Pelajaran
_Avoid_: Registration, Subscription

**Student Status**:
Whether a Student is currently Active, On Leave or Withdrawn.
_Label_: Status Siswa (Aktif / Cuti / Berhenti)
_Avoid_: State

**Class**:
A standing group of Students who study the same Subject at the same Level with one main Tutor.
_Label_: Kelas
_Avoid_: Group, Rombel, Course

**Placement**:
A Student's membership in a Class for a span of time. A Student has at most one current Placement per Subject.
_Label_: Penempatan Kelas
_Avoid_: Assignment, Enrollment

### Teaching

**Session**:
One meeting of a Class on a specific date.
_Label_: Sesi
_Avoid_: Meeting, Pertemuan, Lesson

**Attendance**:
A Student's presence record for one Session: Present, Excused, Sick or Absent.
_Label_: Absensi (Hadir / Izin / Sakit / Alpa)
_Avoid_: Presence, Check-in

**Assessment**:
A scored activity, such as a quiz or test, that measures some or all of a Subject's Competency Aspects. It is separate from a Session.
_Label_: Asesmen
_Avoid_: Test, Exam, Quiz (as general terms)

**Score**:
A number from 0 to 100 given to one Student for one Competency Aspect in one Assessment.
_Label_: Nilai
_Avoid_: Mark, Point

**Tutor Note**:
A Tutor's written comment about a Student's progress in a Subject for an Evaluation Period.
_Label_: Catatan Pengajar
_Avoid_: Remark, Feedback

### Evaluation

**Evaluation Period**:
A named span of dates, defined by the Admin, at the end of which every Student is evaluated and receives a Report Card.
_Label_: Periode Evaluasi
_Avoid_: Term, Semester, Quarter

**Levelling**:
The end-of-period process in which each Student's Level in each Subject is either promoted or retained.
_Label_: Evaluasi dan Levelling
_Avoid_: Promotion, Grading

**Pass Threshold**:
The minimum average Score every Competency Aspect must reach for a Student to be recommended for promotion in a Subject.
_Label_: Ambang Nilai
_Avoid_: KKM, Passing grade

**Minimum Attendance**:
The minimum share of Sessions, counted from the Student's Placement onward, that a Student must attend as Present to be recommended for promotion.
_Label_: Kehadiran Minimal
_Avoid_: Attendance rate requirement

**Level Recommendation**:
The system's suggestion, from Scores and Attendance, to promote or retain a Student in a Subject.
_Label_: Rekomendasi Level
_Avoid_: Auto-promotion, Result

**Incomplete Evaluation**:
A Level Recommendation that cannot be made because at least one Competency Aspect has no Scores in the Evaluation Period.
_Label_: Data Belum Lengkap
_Avoid_: Failed, Missing

**Level Decision**:
The Admin's final ruling for a Student in a Subject: Promote or Retain. It may differ from the Level Recommendation if a reason is given.
_Label_: Keputusan Level (Naik / Tetap)
_Avoid_: Verdict, Pass/Fail

**Level History**:
The record of every Level a Student has held in a Subject and when each change happened.
_Label_: Riwayat Level
_Avoid_: Progress log

**Grade**:
A letter (A, B, C or D) shown on the Report Card for a band of average Scores.
_Label_: Predikat
_Avoid_: Letter grade, Rating

### Reporting

**Report Card**:
A Student's results for one Evaluation Period, covering every Subject they take.
_Label_: Rapor
_Avoid_: Transcript, Progress report

**Publish**:
The Admin's act of releasing a Report Card so the Parent can see it.
_Label_: Terbitkan
_Avoid_: Send, Release, Share

**Combined View**:
A presentation of a Student's progress in all their Subjects side by side. It is not a Level of its own.
_Label_: Tampilan Gabungan
_Avoid_: Overall level, Combined level

**At-risk Student**:
A Student whose Attendance or any Competency Aspect average is currently below the required minimum.
_Label_: Siswa Berisiko
_Avoid_: Failing student, Problem student
