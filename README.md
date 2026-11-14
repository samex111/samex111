<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=rect&color=1B1A17&height=178&section=header&text=Sameer%20Patel&fontSize=48&fontColor=EEE8DC&fontAlignY=40&desc=BACKEND%20ENGINEERING%20%2F%20AI%20SYSTEMS&descColor=C5A46D&descAlignY=68&descSize=14"
    width="100%"
    alt="Sameer Patel — Backend Engineering and AI Systems"
  />

  <img
    src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&duration=3200&pause=1100&color=C5A46D&center=true&vCenter=true&repeat=true&width=820&height=42&lines=Backend+systems+for+AI-powered+products;Governed+agents%2C+retrieval%2C+and+tool+execution;APIs%2C+data+models%2C+and+async+workflows"
    alt="Backend systems for AI-powered products"
  />
</div>

---

## What I build

I work at the intersection of **backend engineering and applied AI**. My focus is the system around the model: the APIs, data layer, retrieval pipeline, tool execution, and asynchronous processing that turn an AI feature into a usable product.

I’m particularly interested in the engineering questions that appear after the first successful demo:

- **Execution boundaries:** What can an agent do, which tools can it access, and when should a human approve an action?
- **Context and retrieval:** Which information should reach a model, how is it retrieved, and how do we keep the result grounded in useful context?
- **Durable workflows:** How should long-running work move through queues, workers, databases, and real-time interfaces without tying everything to one request?

I prefer understanding and designing these boundaries over simply connecting an LLM API to a chat interface.

## Selected engineering work

<a href="https://github.com/samex111/guarded-ai-agent"><img src="https://raw.githubusercontent.com/samex111/samex111/main/assets/guarded-ai-agent.svg" width="100%" alt="01 — Guarded AI Agent" /></a>

**Problem**

An AI agent that can call tools also needs limits. Without a clear execution boundary, tool access, sensitive operations, and the history of an action become difficult to govern.

**System**

I built a policy-governed agent platform in which the policy engine sits between the agent runtime and MCP tools. It supports runtime tool discovery, policy evaluation, approval workflows for sensitive operations, sandboxed file access, and an audit trail. Socket.IO carries execution and approval updates to the interface.

**Engineering focus**

Separating agent orchestration, policy enforcement, and tool execution into explicit parts of the system; coordinating persistent state and background work.

**Stack:** TypeScript · Node.js · Express · MCP · PostgreSQL · Prisma · Redis · BullMQ · Socket.IO · Docker

---

<a href="https://github.com/samex111/web-scrapper"><img src="https://raw.githubusercontent.com/samex111/samex111/main/assets/web-scraper.svg" width="100%" alt="02 — Web Scraper and Lead Intelligence" /></a>

**Problem**

Modern websites often require browser rendering, and scraping several sites should not keep an API request open while the work completes. Raw page data is also less useful than structured information that can be searched and acted on.

**System**

I built an asynchronous scraping platform that separates the API from browser-based workers. Puppeteer handles dynamic pages; the pipeline extracts website metadata, business and contact signals, and social information, then stores structured results for lead analysis and export.

**Engineering focus**

API/worker separation, Redis-backed job queues, browser automation, structured extraction, authentication, and usage controls.

**Stack:** Next.js · Express · TypeScript · Puppeteer · PostgreSQL · Prisma · Redis · BullMQ · Docker

---

<a href="https://github.com/samex111/Accerra"><img src="https://raw.githubusercontent.com/samex111/samex111/main/assets/accerra.svg" width="100%" alt="03 — Accerra Student Intelligence System" /></a>

<sub>In active development</sub>

**Problem**

A test score tells a student how they performed. It rarely explains which prerequisite concept is missing, why a mistake keeps recurring, or whether an idea is actually being retained.

**Product direction**

I’m building Accerra around a different model of student progress: connect concepts and their prerequisites with question attempts, mistakes, and learning signals. The goal is to form a learner-specific picture of understanding and use that context to guide explanations and practice.

The current scope is Physics. I’m working on the knowledge structure and the data model that connects topic-level understanding with a student's learning history. This is an evolving product—not a claim that every planned capability is already shipped.

**Technical direction**

React · TypeScript · Node.js · Express · MongoDB · Mongoose · MongoDB Atlas Vector Search · Gemini

---

<a href="https://www.smjmun.com/"><img src="https://raw.githubusercontent.com/samex111/samex111/main/assets/smjmun.svg" width="100%" alt="04 — SMJMUN Institutional Platform" /></a>

<sub>Client project · Live</sub>

**Problem**

A Model UN organization needs more than a static brochure website. Students need to discover conferences and apply; schools, partners, and volunteers need clear inquiry paths; delegates need a reliable registration journey.

**Delivery**

I designed and developed the public-facing platform around those journeys, including structured conference content, application and inquiry flows, and conference registration/payment integration.

**Stack:** Next.js · TypeScript · Sanity · PostgreSQL · Prisma · Resend · HDFC SmartGateway / Juspay

---

## Engineering toolkit

| Area | Technologies |
|---|---|
| Backend | TypeScript, Node.js, Express, REST APIs |
| Data | PostgreSQL, Prisma, MongoDB, Mongoose |
| Async & realtime | Redis, BullMQ, Socket.IO |
| AI systems | Gemini, RAG, embeddings, vector search, MCP |
| Frontend | React, Next.js, Tailwind CSS |
| Development & deployment | Docker, Docker Compose, Linux, Git |

## What I’m digging into now

- **Retrieval quality:** combining structured knowledge with semantic retrieval, and evaluating whether retrieved context is actually useful.
- **Agent reliability:** keeping model reasoning, tool permissions, policy decisions, and human approvals distinct.
- **Learning models:** representing prerequisite relationships and student understanding as connected data rather than a collection of scores.

---

<div align="center">
  <sub>Building systems with clear boundaries, useful context, and behaviour that can be understood.</sub>
</div>
