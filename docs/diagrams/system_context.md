# System Context Diagram

This diagram shows the system and its external entities.

```mermaid
graph TB
    Builder[Builder / Master]
    Client[Client]
    System[Renovation Planning Platform]
    LLM[AI Service - OpenAI / Gemini]
    ShopAPI[Shop Price API]

    Builder -->|create project, calculate cost, plan work| System
    Client -->|view shopping list, upload receipts, check analytics| System

    System -->|send text for analysis| LLM
    LLM -->|return plan, categories| System

    System -->|request material prices| ShopAPI
    ShopAPI -->|return prices| System