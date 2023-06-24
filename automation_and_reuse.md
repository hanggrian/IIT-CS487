# Automation and reuse

## Automation

| Benefits | Guides |
| :---: | :---: |
| Speed (computers can outperform humans) | Easier if those steps are well
defined. |
| Reliability (computers always follow the rules) | Simple to understand. |
| Robustness (computers never get tired, bored, distracted, frustrated, etc.) | Not likely to change (significantly / frequently) |
| Cost (computers don’t get paid &mdash; per hour, per transaction) | |

### Rapid iteration

| Benefits | Challenges |
| :---: | :---: |
| Reduce the opportunity for change. (customer needs evolve over time, business/competitive demands, technology evolves rapidly) | Difficult to maintain discipline. (the perception is that formal processes take longer, pressure to cut corners) |
| Focus on what is known. (complete understanding is difficult to achieve until we make significant progress, implement what is understood while learning about what should come next) | Overly narrow focus. (each iteration necessarily focuses on the small, new tools, approaches, skills) |
| Everyone wants the system built quickly. (better opportunity to involve the user, less business risk for everyone) | |

### Incremental vs prototyping

| Incremental | Prototyping |
| :---: | :---: |
| Consists of a series of planned (relatively small) efforts designed to result in a complete system to user specification. | Can be used to facilitate incremental development by incrementally improving the prototype into the finished system. |

## Reuse

| Benefits | Drawbacks | Challenges |
| :---: | :---: | :---: |
| Speed, ease of maintenance | **One-size-fits-all** may not be best | Modules must be somewhat generic |
| Peace of mind, reliability, reduced risk | Requires infrastructure (library) and process (check-in/check-out) | Anticipation is key |

### Component models

| Elements | Examples |
| --- | --- |
| Interfaces | Operation names, parameters, exceptions, etc, the appropriate interface definition language (IDL). |
| Information | Naming convention, metadata (data about the component itself), how to customize (configure) for a given deployment. |
| Deployment | How to package the component for deployment. |
