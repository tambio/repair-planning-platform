# Technology Comparison

## 1. Introduction
This document compares technology options for the key parts of the platform. For each decision, we compare 2–3 alternatives and explain the choice.

## 2. Decision 1: Backend Platform

| Option | Pros | Cons |
|--------|------|------|
| Python (FastAPI) | Fast, simple, good for AI and ML, async support | Smaller ecosystem than Node.js |
| Node.js (NestJS) | Good for real-time, one language with frontend | Weaker for AI and data tasks |
| Django (Python) | Full-featured, admin panel, ORM | Heavier, slower for small APIs |

**Choice:** Python (FastAPI)
**Reason:** The project uses AI and OCR. Python has the best libraries for this. FastAPI is fast and simple.

## 3. Decision 2: Frontend Framework

| Option | Pros | Cons |
|--------|------|------|
| React (Next.js) | Big ecosystem, SSR, good for dashboards | More complex setup |
| Vue (Nuxt) | Simple, easy to learn | Smaller ecosystem for enterprise |
| Angular | Full framework, TypeScript | Heavy, slow to start |

**Choice:** React (Next.js)
**Reason:** React is the most popular. Next.js gives server-side rendering and good structure. Many libraries for charts and Gantt.

## 4. Decision 3: Database

| Option | Pros | Cons |
|--------|------|------|
| PostgreSQL + pgvector | Relational, supports vectors for AI, free | Needs setup for vectors |
| MongoDB + Chroma | Flexible schema, good for AI | Two databases, more complex |
| MySQL + Pinecone | Reliable, cloud vector DB | Pinecone is paid, extra service |

**Choice:** PostgreSQL + pgvector
**Reason:** One database for both relational data and AI vectors. Free and reliable. Less complexity.

## 5. Decision 4: AI and LLM

| Option | Pros | Cons |
|--------|------|------|
| OpenAI API | Best quality, easy to use | Paid, needs internet |
| Google Gemini | Good quality, free tier | Limits, needs internet |

**Choice:** OpenAI API + Gemini (fallback)
**Reason:** Best quality for planning and categorization. Gemini as backup. Local model is too heavy for this project.


## 6. Summary Table

| Decision | Choice | Main Reason |
|----------|--------|-------------|
| Backend | Python (FastAPI) | Best for AI |
| Frontend | React (Next.js) | Popular, good for dashboards |
| Database | PostgreSQL + pgvector | One DB for data and vectors |
| AI | OpenAI + Gemini | Best quality |

## 7. Conclusion
The chosen technologies are free or low-cost, well-documented, and fit the project needs. They support AI and scheduling.