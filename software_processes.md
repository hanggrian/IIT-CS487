# Software processes

Process | Roles
--- | ---
Analysis | Gather requirements and understand business goals.
Design | Create software blueprint from the analysis.
Build | Write and compile code from the design.
Verification | Tests and checks to see if final product is acceptable.

## Generic models

| | Waterfall | Incremental | Reuse-oriented
--- | --- | --- | ---
Note | Any engineering effort follows this general approach, but also involves iteration. | Produce a prototype and solicit feedback. | Requires disciplined management of reusable components. (documentation, testing, version control, etc.)
Flow | Cascading from one phase to the next. | Flexiblility to define sub-objective with each iteration. | Prioritize using existing resources.
Pros | Increases the likelihood of true completion. | Evolve methodically, focus on answering questions and resolving challenges. | Faster, defects are limited to points of integration.
Cons | Signoff is required before a phase can be considered complete, makes it difficult to estimate completion time. | &ndash; | Existing components may not exactly match requirements.

| | Spiral | Rational-unified
--- | --- | ---
Note | Iterative, risk driven approach developed by *Barry Boehm*. | Hybrid model incorporating prototyping and incremental delivery. Based on UML and the Unified Software Development Process.
Phases | Objective setting, risk assessment and reduction, development and validation, planning for the next iteration. | Inception, elaboration, construction, transition.

## Agile models

| | Agile | Extreme | XP
--- | --- | --- | ---
Flow | Get a basic idea, then jump into design and implementation cycles. | Rapid development and deployment for small teams and close user involvement. | Test first, then code.
Pros | The benefit is that progress drives discovery which drives more progress. | Requirements come as simple customer stories, change is handled by frequently revisiting. | Similar to analysis and design phases.
Cons | The risk is the discovery is influenced by the working prototype and presence of the customer. | &ndash; | &ndash;
