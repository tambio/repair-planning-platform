# Project Proposal

## Project Title
Development of an intelligent web platform for planning and control of renovation works

## Team Members
- Orman Amir SE2427

## Supervisor
Zhanna Sadirmekova

## Problem Statement
Renovation is a very common task. But today it is not automated well.

People calculate costs in Excel or on paper. The work schedule is only in the builder's head. Receipts are lost. Extra spending is found too late.

This causes:
- delays in time,
- spending more money than planned,
- conflicts between the client and the builder.

Existing apps are either too small (only cost calculation) or too big (corporate systems). They are not good for small private teams.

## Target Users
1. **Private builders and masters** — they need fast cost calculation, work planning, and money control.
2. **Clients (people who do renovation)** — they want to know what to buy, when to buy, and how much money is already spent.

## Aim
Develop a web platform for planning and control of renovation works. The platform calculates costs, builds a work schedule, and tracks real spending.

## Objectives
1. Study the domain: types of renovation work, material usage norms, and how clients and builders work together.
2. Design the platform architecture: modules for costs, planning, shopping list, receipts, and analytics.
3. Develop a module for automatic cost calculation and material list creation.
4. Implement an AI module for scheduling. It must consider dependencies between works, technical pauses, and worker availability.
5. Develop a module for expenses: upload receipts, OCR recognition, and automatic category assignment.
6. Implement an analytics module: plan vs fact for time and budget.
7. Test the platform and evaluate the AI modules.

## Expected Outcomes
**Software product:**
- Web platform with separate accounts for builder and client.
- Cost module: calculates materials and prices by work type.
- AI planner: builds a Gantt chart with dependencies and pauses.
- Client portal: shopping list by renovation stages.
- Receipt module: photo upload, OCR, and expense categorization.
- Analytics dashboard: plan vs fact for budget and time, forecast of final cost.

**Documentation:**
- Final report with architecture and algorithm explanation.
- User guide.
- Test results and evaluation of AI modules.

## Project Scope

### In scope:
- Cost calculation by work type and area.
- Material list creation.
- Work schedule with dependencies and pauses.
- Real expense tracking based on receipts.
- Analytics: plan vs fact for budget and time.
- AI modules: planner, receipt OCR, expense categorization.

### Out of scope:
- The renovation work itself.
- Buying and delivering materials.
- Legal support.
- Integration with banks and accounting systems.
- Mobile app (only responsive web interface).

## Selected Technologies
- **Backend:** Python (FastAPI)
- **Frontend:** React (Next.js) + Tailwind CSS
- **Database:** PostgreSQL + pgvector
- **AI:** OpenAI API / Gemini, LangChain
- **OCR:** Tesseract / Google Vision API
- **Planning:** OR-Tools
- **Project management:** GitHub + YouTrack

## Current Status
Analysis and design stage. Prepared: proposal, requirements, architecture diagrams, verification plan.