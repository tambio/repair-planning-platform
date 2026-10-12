# Component Diagram (Draft)

This diagram shows the main components of the system.

```mermaid
graph TB
    subgraph Frontend
        UI_Builder[Builder Dashboard]
        UI_Client[Client Dashboard]
        UI_Auth[Login / Register]
    end

    subgraph Backend
        API[API Gateway - FastAPI]
        Auth[Auth Service]
        Cost[Cost Calculation Module]
        Planner[AI Planning Module]
        Receipts[Receipt Module]
        Analytics[Analytics Module]
        Notify[Notification Service]
    end

    subgraph Data
        DB[(PostgreSQL)]
        Vector[(pgvector - AI Vectors)]
        Files[File Storage - Receipts]
    end

    subgraph External
        LLM[OpenAI / Gemini]
    end

    UI_Builder --> API
    UI_Client --> API
    UI_Auth --> API

    API --> Auth
    API --> Cost
    API --> Planner
    API --> Receipts
    API --> Analytics
    API --> Notify

    Auth --> DB
    Cost --> DB
    Planner --> DB
    Planner --> Vector
    Planner --> LLM
    Receipts --> DB
    Receipts --> Files
    Analytics --> DB
    Analytics --> Vector