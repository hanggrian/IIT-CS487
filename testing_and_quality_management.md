# Testing and quality management

## Quality

| Quality Assurance | Quality Control |
| :---: | :---: |
| Quality Assurance | Prevent defects, improve the level of quality through an efficient set of activities performed throughout the life cycle. | Eliminate defective products, improve the rate of acceptable product delivery through an efficient set of defect detection activities, primarily late in the life cycle. |

### Perform quality control

| Action | Description |
| --- | --- |
| Feedback loops | Measure the output of a process, as compared to expected, understand the results (both good and bad), use that knowledge to improve the process. |
| Root-cause analysis | Ask yourself what caused a problem to occur, then ask what caused that cause, and so on. |
| Histograms and Pareto Charts | Frequency of problems by problem category, 80% of the problems are due to 20% of the causes, invest in eliminating the most problematic causes. |

### Cleanroom software engineering

Target is zero-defect software. Keep the development environment **ultra
clean**.

- Formally specify the system showing system response to stimuli. (state
  transitions)
- Utilize incremental development with significant user involvement.
- Rely on structured programming and limit the use of control and data
  abstraction.
- Rigorous software inspections.
- Statistical testing to determine reliability.

### Configuration management

*Configuration management (CM)* supports the evolution of software systems
through a progression of versions. (policies, processes, and tools)

| Type | Description | Implementation |
| --- | --- | --- |
| Change management | Change happens (mainly for good), change requests (formality reduces risk and impact), decision making (change control board). | Project planning and documentation, timing, cutover and rollback. |
| Version management | Inevitable evolution often results of multiple **supported** versions | Branching and merging. |
| System building | Compiling and linking the latest checked in components into a version of the system | Build script generation, VM system integration, minimal recompilation, executable system creation, test automation, reporting, documentation generation. |
| Release management | A package for distribution. (major for new functionality and minor for patches) | Current system quality, platform changes, new-feature release, competition, marketing commitments, custom changes. |

## Testing

| Testing | Inspections |
| :---: | :---: |
| Defects can **hide beneath** other defects, requires a certain degree of completeness. | Can look at other important factors beyond correctness. (portability, maintainability, efficiency, etc.) |

### Development testing

| Granularity | Description |
| --- | --- |
| Unit testing | Exercise the functionality of logical units of the system. |
| Component testing | Verify proper operation of interacting entities such as objects. |
| System testing | Exercise the system as a whole for proper operation, exception handling, tolerance of load, etc. |

### Release testing

| Type | Description |
| --- | --- |
| Requirements testing | Requirements should be testable, demonstrate proper implementation of system requirements. |
| Scenario testing | Verify **realistic** operation. |
| Performance testing | &ndash; |

### User testing

| Approach | Description |
| --- | --- |
| Alpha | Within development process. |
| Beta | **Field** testing of a preliminary release. |
| Acceptance | Users determine **fitness**. |

### Interface testing

| Type | Description |
| --- | --- |
| Box testing | Predictable output for given input, **correctly incorrect** output for given improper input. |
