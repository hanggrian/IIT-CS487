# Requirements engineering

| Type | Description |
| --- | --- |
| Functional | Describe what the system should do, how the system should react to certain inputs, how the system should behave in certain situations. |
| Non-functional | Constraints on the services or functions offered by the system, often apply to the system as a whole (not directly concerned with specific functions), system performance, security, availability, etc. |
| Domain | Derived from the system’s domain. |

| Type of non-functional | Description |
| --- | --- |
| Product | Execution speed, memory requirements, acceptable failure rate, portability, usability, etc. |
| Organizational | Policies, procedures, process standards, programming languages, methodologies, tools, devlivery timeframe, etc. |
| External | Interoperability with other systems, legal requirements, ethical requirements, etc. |

## Capturing requirements

### User requirement challenges

| Challenge | Description |
| --- | --- |
| Ambiguity | Clarity is difficult to achieve, especially since brevity is also desirable, human language is different than user language is different than system language. |
| Confusion | Functional vs non-functional vs system goals vs design information, confusion over how/where to capture requirements can lead to documentation issues. |
| Amalgamation | A single stated requirement may actually contain several requirements. |

### System requirements challenges

- Although undesirable, some design / implementation language may be necessary.
  (architecture, interoperability, etc.)
- Natural language is ambiguous and allows for saying the same thing in multiple
  distinct ways.
- Relating related requirements is difficult using natural language.

### Specific notations

| Notation | Example |
| --- | --- |
| Scructure natural language | Human language with standard forms / templates. |
| Design description languages | Including pseudo-code. |
| Graphical notations | Flowcharts, use-case, sequence diagrams, etc. |
| Mathemathical specifications | Based on mathematical concepts such as finite-state machines or sets. |

### Requirements document

| Section | Subsections |
| --- | --- |
| Introduction | Preface, background, glossary. |
| Content | User requirements, system architecture, system requirements, system models, system evolution. |
| Conclusion | Appendices, index. |

## Engineering of requirements

The goal is to create and maintain a system requirements document.

| Steps | Outputs | Discussion |
| --- | --- | --- |
| Feasibility study | Feasibility report | Should we build it? Are we currently capable of building it? Can we become capable of building it? etc. |
| Requirements elicitation and analysis | System models | Working with stakeholders to **discover** requirements, challenges, and process. |
| Requirements specification | User and system requirements | Understanding multiple viewpoints, interviewing stakeholders, capturing scenarios, use-cases. |
| Requirements validation | Requirements document | A checkpoint for ensuring that the requirements as specified truly define the system the customer wants, a gate that should not be passed without a fight, things to look for. (clarity, consistency, etc.) |
