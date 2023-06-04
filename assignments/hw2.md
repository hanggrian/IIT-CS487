# [Homework 2](https://github.com/hendraanggrian/IIT-CS487/blob/assets/assignments/hw2.pdf)

## Problem 1

> Consider an automated exam system.
>
> Describe test cases to prove the system satisfies each of the following
  requirements (you may improve the requirements in any way you see as
  necessary):

### Subproblem 1A

> “The system must accept responses such that the system is fully aware of the
  student’s intent for each response”.

Protecting against cheating has always been a challenge in any exam, even more
so in an automated environment where there is little or no human supervision. As
a safeguarding effort, the tests should demonstrate that the system could
distinguish malicious attempts and good intentions during ongoing exams.

**Test cases**:

- Divert application focus &mdash; Warn the user and log the incident.
- Access prohibited websites &mdash; Abruptly end the exam and report the
  incident.
- Close the application before submission &mdash; Prohibits the user from coming
  back to this exam. Stopping the monitoring session (purposely or not) allows
  the user to cheat under detection. There should have been a clear warning
  about not losing internet access during the exam.

### Subproblem 1B

> “The system must grade all exam questions quickly”.

Swiftness in grading is a tricky requirement considering correct assessment is
deemed more important than how fast they can be produced. The system is also at
a disadvantage in processing all submissions at once, adding more stress to the
grading capability.

**Test cases**:

- Submit a lot of answers &mdash; Grading should be finished within a rational
  time given that their difficulty is reasonable, preferably on the same day.
- Submit complex answers &mdash; Throw a curve ball to the system by submitting
  answers with varying degrees of difficulty. See if the elapsed time is
  comparable with the first case.

### Subproblem 1C

> “The system must accurately assess the student’s awareness of course
  material”.

I would relate course material awareness to student's academic comprehension and
therefore directly affects the scoring system. To measure such comprehension,
the test could validate student answers with known correct truths from the
latest knowledge base.

**Test cases**:

- Test the tester &mdash; Consult the grades produced by the automated system
  with experts in the respective fields.

## Problem 2

> Propose an HCI “protocol” to satisfy the above and explain how each part
  addresses the requirements:
>
> - C &rarr; H: Describe how questions are presented to the student.
> - H &rarr; C: Describe how the students will submit their responses.

### Subproblem 2A

> “The system must accept responses such that the system is fully aware of the
  student’s intent for each response”.

Split the question sheet into sub-sections and track students' movement in each
section. Malicious intent like copy-pasting from other sources is to be noted.

### Subproblem 2B

> “The system must grade all exam questions quickly”.

Instead of waiting for users to submit the whole paper, the system can start
pre-calculating the scores as users enter their input. For example, when a
student moves to the next question, assign a score to the previous answer and
use it unless the user goes back to the initial question.

### Subproblem 2C

> “The system must accurately assess the student’s awareness of course
  material”.

Validate student answers with content from lectures given earlier.
