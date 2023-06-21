# Modeling and design

## Models

| Purpose | Perspectives |
| :---: | :---: |
| Words have limited effectiveness | External context |
| A picture can say a thousand words | System behavior |
| Bridge the gap from analysis to design | Architecture |

### Context models

| Boundaries | Interfaces |
| :---: | :---: |
| Where does the system end and its surrounding environment begin? Similar to in-scope vs out-of-scope, not necessarily dictated by technical constraints. | Are related components within the boundaries or accessible via defined interfaces? |

### Interaction models

| Type | Description |
| --- | --- |
| Use case modeling | Each represents a discrete external interaction, very high level (narrative is needed for detail). |
| Sequence diagrams | Captures a sequence of interactions, the sequential flow of a given use case. |

### Structural models

| Type | Description |
| --- | --- |
| Class diagrams | Object-oriented classes and how they are associated, model the **real world**. |
| Generalization hierarchy | Use more general terms to avoid getting **caught** in the details, members have common characteristics. |
| Aggregation association | Building components from sub-components. |

### Behavioral models

| Type | Description | Discussion |
| --- | --- | --- |
| Data-flow models | Work is often driven by information flowing through an organization and the manner in which the organization processes, consumes and disseminates it. | Where does the information come from? Who owns it? How is it processed?, etc. |
| Event-driven (state machine) models | Organizations move from state to state due to some sort of stimulus | How will the system react to different events? Who or what will cause each event? etc. |

### Data models

| Type | Description |
| --- | --- |
| Data dictionary | Alphabetic listing of data entities and their descriptions, helps manage the abstract nature of representing the real world in a system design. |

## Design patterns

| Configuration management | Host-target development |
| :---: | :---: |
| Version control | Configure development host to match target |
| System build management | Simulate target for testing |
| Issue management | |

### Architectural views

| View | Description |
| --- | --- |
| Logical | The system as interacting objects. |
| Process | Interacting processes. |
| Development | Interacting processes. |
| Physical | Interacting hardaware and software. |
| Conceptual | The basis for decomposing high-level requirements. |

### Architectural patterns

| Architecture | Description |
| --- | --- |
| Layered architecture | Achieve separation and independence through layering, hierarchical organization, supports incremental development. |
| Repository architecture | Support the exchange of information between sub-systems, use a central repository to manage shared data, establish and maintain a separate database for each sub-system. |
| Client-server architecture | Organized as a set of services and associated servers, accessed by clients **calling** the services. |
| Pipe-and-Filter architecture | Workflow, information is transformed as it flows through the system. |

| Generic-layered architectures | Application architectures |
| :---: | :---: |
| User interface | Alternatives to system architectures that focus on the needs of the application |
| User interface management, authentication and authorization | Data-processing applications |
| Core business logic/application functionality, system utilities | Transaction-processing applications |
| System support. (OS, database, etc.) | Event-processing systems |
| | Language-processing systems |

### Modular decomposition styles

| Style | Description |
| --- | --- |
| Object-oriented decomposition | Loosely coupled objects with well defined interfaces, classes are templates with attributes and operations, during execution, objects are instantiated from classes. |
| Function-oriented pipelining | Data flow, inputs are processed by transformational functions to produce outputs. |

### Control styles

| Style | Description |
| --- | --- |
| Centralized control | Design a sub-system whose primary function is to control the other sub-systems, the vast majority of control is handled by this sub-system. |
| Event-based control | Design each sub-system to **react** to events, events can come from other sub-systems or the environment. |

### Distributed systems

| Benefits | Disadvantages |
| :---: | :---: |
| Shared and therefore better utilized resources | Complexity |
| Open and therefore more standard-driven systems | Vulnerable to security breaches |
| Concurrency | Difficult to manage |
| Scalability | Unpredictability |
| Fault tolerance | |

| Type | Description |
| --- | --- |
| Multiprocessor architectures | The operating system *can* distribute the processes of a software system across multiple processors, the processes must be capable of running independent of each other. |
| Client-server architectures | A centralized server system “offers” services to de-centralized client processes. (thin-client and fat-client systems) |

| Pattern | Description |
| --- | --- |
| Master-slave architecture | Real-time systems requiring guaranteed response times. |
| 2-tier client-server architecture | Centralized systems for security reasons. |
| Multi-tier C/S architecture | To support high-volume transaction processing. |
| Distributed component architecture | Supports combining resources from different systems. |
| Peer-to-peer architecture | Servers **introduce** peers who then work together locally. |
