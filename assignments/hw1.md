# [Homework 1](https://github.com/hendraanggrian/IIT-CS487/blob/assets/assignments/hw1.pdf)

## Problem 1

> Describe the purpose of each of the following phases: analysis, design, build,
  verify, release, maintenance.

### Analysis

The analysis marks the beginning of a software development lifecycle, the whole
purpose being problem identification and coming to an agreement with responsible
parties. The production team is expected to be guided by end users during this
phase. However, the amount of time required for said activities usually depends
on the team's familiarity with the subject. The final report of the analysis
phase should also include less-mutable requirements.

### Design

In the design phase, the production team lay out a blueprint based on the
requirements formulated from the analysis phase as guidelines. The blueprint is
then conceptualized using visualization, and eventually, a working graphical
prototype.

### Build

The building is where the actual code production begins, which amounts to
deviating algorithms, creating the database, network connection to the
application, appling security layers, and other activities based on how complex
the requirements are. It is arguably the most difficult cycle considering the
written code should be production-ready.

### Verify

The verification refers to ensuring source code integrity by testing, which
itself is divided into sub-categories unit testing, functional testing,
integration testing, and others. This feature can be further extended with code
styling checks, also known as linter.

### Release

Releasing means delivering the product to its final destination, be it end-user,
online services, or any entity. This phase is trickier when the software in
question is proprietary. In such a case, an exposed executable or source code
would be wholly unacceptable, leaving the production team with a limited mode of
code transportation.

### Maintenance

As the software initially deployed is being in use, certain issues might arise
in the process. They are likely newly encountered bugs that obviously slid
through the verification phase, security breaches, or general quality-of-life
improvement. These are the common tasks performed during the maintenance phase.

## Problem 2

> Every development effort will end with UAT - explain.

UAT is a type of test performed in the presence of the users, acting as a grant
of approval between them and the production team. The tests are ordinarily
undertaken in the final phase of the development stages as prerequisites for
such approval.

Due to this pretext of agreement between two parties, UAT is often included in
contracts and therefore becomes legally binding.

## Problem 3

> Consider the iterative approach.

### Subproblem 3A

> Explain why it is logical to assume that each iteration will bring the
  development closer to 100% successful completion.

The iterative approach is a software design methodology that revolves around
flexibility by allowing each phase to run consecutively with another. By
removing the ordered chain of command, the production team can theoretically go
straight to prototyping and inciting feedback from users.

And though the prototype is flawed, it serves as the proof of work most visible
to the users. It incites feedback and tells the producer what to fix and/or
refine in the next iteration. Therefore, it is logical that each iteration will
bring the final product to perfect completion.

### Subproblem 3B

> Give one reason why this desired continuous progress may not happen and
  describe a way to ensure that it will.

Nevertheless, the always-updating nature of the requirements in the iterative
design model can bring extra cost and overhead, which could spiral into an
endless cycle without adequate supervision. The development process can also be
stalled when there are multiple solutions not aligning with one another, thereby
indicating confusion within the team.

To prevent (or at least constraint) changes, it's best to break the requirements
apart into smaller pieces so that they can be easily tracked and flagged for
deadlines.

### Subproblem 3C

> Explain why the iterative approach may take longer to complete than the
  schedule allows and describe a way to minimize this possibility.

The way iterative design methodology works is by completing each cycle
successively, which takes a toll on the schedule. One of the tools available to
solve this dilemma is applying incremental build standardization.

Incremental build refers to sub-sections of the project, usually version-coded.
It enables production team to use them as knowledgebase and run consecutively
with other iterations.
