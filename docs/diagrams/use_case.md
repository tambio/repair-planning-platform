# Use Case Diagram

This diagram shows what users can do in the system.

```mermaid
graph LR
    Builder((Builder))
    Client((Client))

    UC1[Register / Login]
    UC2[Create Project]
    UC3[Calculate Cost]
    UC4[View Material List]
    UC5[Build Schedule with AI]
    UC6[View Gantt Chart]
    UC7[View Shopping List]
    UC8[Upload Receipt]
    UC9[Enter Expense Manually]
    UC10[View Plan vs Fact Analytics]
    UC11[Forecast Final Cost]

    Builder --> UC1
    Builder --> UC2
    Builder --> UC3
    Builder --> UC4
    Builder --> UC5
    Builder --> UC6

    Client --> UC1
    Client --> UC7
    Client --> UC8
    Client --> UC9
    Client --> UC10
    Client --> UC11