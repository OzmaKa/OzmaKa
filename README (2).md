<div align="center">

---

## `whoami`

I'm Oussamah, a software engineer focused on full-stack development and AI-augmented systems.

I work primarily with **TypeScript, React, Node.js, and Python**, while building toward deeper expertise in **RAG systems, agentic AI, LLM evaluation, and developer tooling**.

I care about shipping software that actually works in production — with validation, observability, security, and maintainability treated as part of the engineering problem.

Some things I've shipped:

- 🩺 **React Doctor** — React performance CLI with [![npm downloads](<https://img.shields.io/npm/dt/react-doctor-cli-dev?style=flat-square&label=npm%20downloads&color=brightgreen>)](https://www.npmjs.com/package/react-doctor-cli-dev) 
- 🤖 **CodeShift** — AI code converter and reviewer with SSE streaming and structured outputs
- 🔎 **RAG systems** — Cohere embeddings, ChromaDB, LangChain, LCEL, and LangSmith
- 🧠 **Agent systems** — multi-step tool calling with evaluation and red-team testing
- 🔐 **Instagram Vault** — privacy-first React application with zero server-side data storage

---

## `currently`

```yaml
shipping:
  - React Doctor       # React performance CLI · static analysis + runtime profiling
  - CodeShift          # AI code converter + reviewer · SSE + structured outputs
  - Instagram Vault    # Privacy-first archive app + Chrome extension

available:
  - Remote AI engineering
  - Full-stack engineering
  - Contract work
  - Open-source collaboration
```

---

## 🩺 React Doctor

### React Performance Profiler & Static Analyzer

React Doctor is a CLI-based React performance analysis tool that combines **Babel AST static analysis**, **real-browser runtime profiling**, and an intelligent **rule engine** to identify performance problems and generate actionable fix suggestions.

It doesn't just look for code patterns.

It connects static findings with runtime evidence to help distinguish potential problems from issues that actually affect application behavior.

### What it does

- 🔍 AST-based JSX/TSX static analysis
- 🌐 Real-browser runtime profiling
- ⚡ Core Web Vitals measurement
- ♻️ React render and commit analysis
- 🧠 Cross-referenced performance rules
- 💡 Human-readable explanations and fix suggestions
- 📊 Structured JSON reports
- 🖥️ CLI + dashboard workflow
- 📱 Desktop and mobile simulation

### Proof of shipping

[![npm version](https://img.shields.io/npm/v/react-doctor-cli-dev?style=flat-square)](https://www.npmjs.com/package/react-doctor-cli-dev)
[![npm downloads](<https://img.shields.io/npm/dt/react-doctor-cli-dev?style=flat-square&label=total%20downloads&color=brightgreen>)](https://www.npmjs.com/package/react-doctor-cli-dev)

### Quick start

```bash
npx react-doctor-cli-dev full ./
```

### Links

[🌐 Website](https://react-doctor-cli.web.app) · [📦 npm](https://www.npmjs.com/package/react-doctor-cli-dev) · [💻 GitHub](https://github.com/softar-dev/React_Doctor)

* [ ] Example

```js
const result = await analyze('./src')

// ⚠ 3 issues detected

result.issues.forEach(issue => {
  console.log(issue.suggestion)
})

// ✓ Report generated
```

**Stack:** Node.js · TypeScript · Babel AST · Puppeteer · CLI · Monorepo · Static Analysis

---

## `projects`

### 01 — CodeShift

#### AI Code Converter & Reviewer

A full-stack AI application that converts and reviews source code using Cohere's LLM.

Features include:

- SSE streaming for real-time output
- Zod-validated structured JSON responses
- Code quality scoring, issue detection and suggestions
- Production-hardened Express backend
- Rate limiting, request logging, health checks, input validation

**Stack:** React · TypeScript · Node.js · Express · Cohere API · Zod · Firebase · Render

[GitHub](https://github.com/OzmaKa/Code-Shift) · [Live Demo](https://code-shift-dev.web.app/)

---

### 02 — Multi-Step Agent & Evaluation Harness

#### Tool-calling agent with evaluation and security testing

A persistent multi-step agent that chains tool calls across multiple iterations until a task is complete.

Includes a full evaluation harness:

- Condition-based test suites
- LLM-as-judge evaluation (helpfulness + accuracy scoring)
- Red-team adversarial + prompt-injection testing
- Safe math evaluation using Python's `ast` instead of `eval()`

The security evaluation discovered and fixed **two prompt injection vulnerabilities** before deployment.

**Stack:** Python · Cohere · Pydantic · Function Calling · Agents · LLM Evaluation · Red-teaming

[GitHub](https://github.com/OzmaKa/structured-output)

---

### 03 — RAG Pipeline · Document Q&A

#### Retrieval-Augmented Generation from First Principles

A from-scratch RAG pipeline built to understand the fundamentals behind modern retrieval systems.

The pipeline:

1. Chunks documents into paragraphs with overlap
2. Generates 1024-dimensional Cohere embeddings
3. Stores vectors in ChromaDB
4. Performs semantic retrieval
5. Generates grounded answers from retrieved source content

A LangChain version extends the system with LCEL composition and LangSmith tracing.

**Stack:** Python · Cohere · ChromaDB · Vector Search · Embeddings · LangChain · LCEL · LangSmith

[GitHub — from scratch](https://github.com/OzmaKa/rag-project) · [GitHub — LangChain](https://github.com/OzmaKa/langchain-rag)

---

### 04 — Instagram Vault

#### Privacy-First Instagram Saved-Post Archive

A React application that parses an official Instagram data export and creates a fully searchable and filterable archive of saved posts and reels — all data stays inside the browser, zero server-side storage.

Includes a companion Chrome extension that captures saves while scrolling.

Features: IndexedDB storage · Search & filtering · Collections · Tags · Favorites · CSV/TXT/JSON export · Lazy-loaded link previews · Chrome extension integration

**Stack:** React · TypeScript · Vite · Zustand · IndexedDB · SCSS · JSZip · Chrome Extension API

[Live Demo](https://instagram-vault.web.app/)

---

### 05 — MUGI CSS Library

#### Lightweight CSS Component Library

A CSS library sitting between Bootstrap's component-heavy approach and Tailwind's utility-first model — built entirely from scratch with predefined component classes, theme support, and a clean SCSS architecture.

**Stack:** CSS3 · SCSS · Design Systems · Theming

[GitHub](https://github.com/OzmaKa/MUGI.git) · [Live Demo](https://mugi-css.web.app/)

---

### 06 — Three.js Earth

#### Interactive 3D Earth

Realistic textures · Atmospheric glow · City lights · Smooth orbit controls · WebGL rendering

**Stack:** Three.js · WebGL · JavaScript · GLSL Shaders

[GitHub](https://github.com/OzmaKa/Three.js-Earth.git)

---

## `stack`

```text
Languages     TypeScript · JavaScript · Python · Java · C++ · SQL · MATLAB

Frontend      React · Three.js · HTML5 · CSS3 · SCSS · PWAs · Responsive Design

Backend       Node.js · Express · REST APIs · SSE · Authentication · Rate Limiting

Databases     PostgreSQL · MongoDB · ChromaDB · IndexedDB
              Views · Triggers · Indexes · Transactions

AI / LLM      Cohere API · LangChain · LCEL · RAG · Embeddings · Vector Search
              Multi-step Agents · Function Calling · Structured Outputs
              Zod · Pydantic · Prompt Engineering
              LLM Evaluation · LLM-as-Judge · Red-teaming · LangSmith

DevTools      Babel AST · CLI Design · Monorepos · Git · GitHub
```

---

## `engineering`

I care about more than getting a demo to work.

```text
Correctness → Validation → Observability → Security → Evaluation → Maintainability → Production
```

That means: structured outputs over free-form responses · input validation at API boundaries · rate limiting and request logging · health checks · LLM evaluation · red-team and prompt-injection testing · runtime profiling · static analysis · type-safe interfaces · reproducible workflows.

---

## `stats`

<div align="center">

---

## `numbers`

<table>
<tr><td>📦 React Doctor downloads</td><td><a href="https://www.npmjs.com/package/react-doctor-cli-dev"><img src="https://img.shields.io/npm/dt/react-doctor-cli-dev?style=flat-square&color=brightgreen" /></a></td></tr>
<tr><td>🚀 Projects shipped</td><td><strong>9+</strong></td></tr>
<tr><td>💼 Status</td><td><strong>Open to remote opportunities</strong></td></tr>
</table>

---

## `reach me`

Open to remote AI engineering · full-stack engineering · contract work · open-source collaboration.

```text
Portfolio  →  https://oussamah-kabalan.netlify.app
LinkedIn   →  https://linkedin.com/in/oussamah-kabalan-9618923a
GitHub     →  https://github.com/OzmaKa
```

---

<div align="center">
