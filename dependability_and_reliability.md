# Dependability and reliability

## Dependability

| Consideration | Description |
| --- | --- |
| Repairability | The ability to recover from failure, diagnosis, analysis, “surgical” repair, etc. |
| Maintainability | Economical adaptation to new requirements. |
| Survivability | The ability to withstand **attack**, recognize, resist, and recover. |
| Error tolerance | Avoid or at least tolerate user errors, autocorrect if possible, teach the user along the way. |

### Safety-critical systems

| Level | Description |
| --- | --- |
| Primary safety-critical systems | Embedded system controllers, failure of the controller leads to failure of the system it is controlling. |
| Secondary safety-critical systems | Failure of this system will not directly cause harm, however such a failure could lead to harmful situations. (e.g., CAD or CASE tools) |

## Reliability

### Security management

| Type | Description |
| --- | --- |
| Access | User and permission management, restrict users' access. |
| Deployment | Control installation and configuration, patching. |
| Attacks | Monitoring, detection, and recovery. |

### Maintenance activity

| Driver | Description |
| --- | --- |
| Interfaces | Number and complexity matter, user and system interfaces. |
| Information | Number of data sources, data structure complexity. |
| Volatile requirements | Policies and procedures, business rules, technology. |
| Processes utlizing the system | The more users, the more demand for change. |

### Refractoring

| Goals | Targets |
| :---: | :---: |
| Improve structure and performance | Removal of duplicate code |
| Reduce complexity | Decomposing long methods |
| Improve understandability | Simplify or replace **switch** statements |
| | Encapsulate recurring **clumps** of data |
| | Remove speculative generality |

### Legacy systems

| Justification | Next steps |
| :---: | :---: |
| Change is risky | Scrap it |
| Need downtime to switch over | Leave it as is and maintain |
| Domain knowledge seeps away over time | Reengineer it to improve maintainability |
| | Replace all or at least some of it |
