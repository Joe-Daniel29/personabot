# AI Mentor Hub

A persona chatbot built to provide specialized guidance. Switch between three domain experts:

- **Alice** — Frontend Architect. Specializes in React, UI/UX, and accessibility.
- **Bob** — Backend Wizard. Node.js, microservices, databases, and system design enthusiast.
- **Charlie** — Data Scientist. Python, ML models, stats. Focuses on data quality and insights.

Each persona has its own deeply-crafted system prompt with a persona description and specific behavior traits. Switching personas resets the conversation so you always start clean.

---

## Setup

```bash
# 1. Clone & install
git clone <your-repo>
cd personabot
bun install     # or: pnpm i / npm i / yarn

# 2. Configure your API key
cp .env.example .env.local
# Open .env.local and paste your Gemini API key.

# 3. Run
bun dev         # or: npm run dev
# → http://localhost:3000
```

---

## Project structure

```
src/
├── app/
│   ├── api/chat/route.ts
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components/
│   ├── ChatInterface.tsx
│   ├── PersonaSwitcher.tsx
│   ├── PersonaAvatar.tsx
│   ├── MessageBubble.tsx
│   ├── SuggestionChips.tsx
│   └── TypingIndicator.tsx
├── data/
│   └── personas.ts
└── lib/
    └── types.ts
.env.example
prompts.md
reflection.md
```
