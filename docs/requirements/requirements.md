# Requirements Specification

## 1. Introduction
This document describes the functional and non-functional requirements for the intelligent web platform for renovation planning and control.

## 2. Functional Requirements

### FR-01: User registration and login
The system must allow users to register and log in.
- Priority: Must
- Acceptance criteria: User can create an account and log in with email and password.

### FR-02: Two user roles
The system must have two roles: builder and client.
- Priority: Must
- Acceptance criteria: Each role sees its own interface and functions.

### FR-03: Create renovation project
The builder must be able to create a new renovation project.
- Priority: Must
- Acceptance criteria: Builder enters project name, address, area, and type of work.

### FR-04: Cost calculation
The system must calculate the cost of renovation works.
- Priority: Must
- Acceptance criteria: System calculates materials and price by work type and area.

### FR-05: Material list
The system must create a list of materials for the project.
- Priority: Must
- Acceptance criteria: List shows material name, quantity, and price.

### FR-06: Work schedule (AI)
The system must build a work schedule automatically using AI.
- Priority: Must
- Acceptance criteria: Schedule considers dependencies between works and technical pauses.

### FR-07: Gantt chart
The system must show the schedule as a Gantt chart.
- Priority: Should
- Acceptance criteria: User can see all tasks on a timeline.

### FR-08: Shopping list for client
The system must show a shopping list for the client.
- Priority: Must
- Acceptance criteria: Client sees what to buy now and what to buy later.

### FR-09: Receipt upload
The client must be able to upload photos of receipts.
- Priority: Must
- Acceptance criteria: User can upload a photo and the system saves it.

### FR-10: OCR receipt recognition
The system must read text from receipt photos using OCR.
- Priority: Should
- Acceptance criteria: System extracts store name, date, total amount, and item list.

### FR-11: Expense categorization
The system must group expenses by category.
- Priority: Should
- Acceptance criteria: Each item from the receipt gets a category (e.g., tiles, glue, paint).

### FR-12: Plan vs fact analytics
The system must show analytics: plan vs fact for budget and time.
- Priority: Must
- Acceptance criteria: User sees planned cost, real cost, and difference.

### FR-13: Expense forecast
The system must forecast the final cost of the renovation.
- Priority: Could
- Acceptance criteria: System shows predicted total cost based on current spending.

### FR-14: Notifications
The system must notify users about important events.
- Priority: Could
- Acceptance criteria: User gets a notification when a task is delayed or budget is exceeded.

## 3. Non-Functional Requirements

### NFR-01: Performance
The system must respond to user actions in less than 2 seconds.
- Priority: Must

### NFR-02: Security
User data must be protected. Passwords must be hashed.
- Priority: Must

### NFR-03: Responsive design
The interface must work on desktop and mobile devices.
- Priority: Should

### NFR-04: Usability
The interface must be simple and clear for non-technical users.
- Priority: Must

### NFR-05: Reliability
The system must work at least 99% of the time.
- Priority: Should

### NFR-06: Scalability
The system must support at least 1000 users without performance loss.
- Priority: Could

## 4. Priorities
- **Must** — required for MVP.
- **Should** — important but can be added later.
- **Could** — nice to have, added if time allows.

## 5. Acceptance Criteria Summary
All "Must" requirements must be tested and confirmed before the final defense.