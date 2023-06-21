# Service-oriented architecture and embedded software

## SOA-related standards

| Standard | Description |
| --- | --- |
| *SOA Protocol (SOAP)* | Message interchange, supports communication between services. |
| *Web Services Definition Language (WDSL)* | Service interface definition, establishes definition for service operations and bindings. |
| *Web Services Business Process Execution Language (WS-BPEL)* | Workflow language. |

### Service types

| Type | Description | Example |
| --- | --- | --- |
| Utility services | General functionality. | Currency conversion. |
| Business services | Associated with a specific business function. | Student registration. |
| Coordination of process services | Support more general business processes. | Procurement process management. |

## Embedded software

### Real-time design patterns

| Pattern | Examples |
| --- | --- |
| Observe and react | Sensors are monitored and status displayed, sensor change initiates handler. |
| Environmental control | Sensors monitor the environment and actuators adjust it, Sensor change initiates signals to actuators. |
| Process pipeline | Data transformation is required before processing, separate processors to handle concurrent transformations. |

### Timing analysis factor

| Factor | Description |
| --- | --- |
| Deadlines | The time by which stimuli must be processed. |
| Frequency | The number of times per second that a process must execute. |
| Execution time | The time required to process a stimulus and produce a response (consider both average and worst case). |
