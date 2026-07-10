# Pitch Agent Architecture

## Multi-Agent AI System

This document provides a high-level overview of Pitch Agent's public system architecture.

Pitch Agent is designed as a modular multi-agent AI system that orchestrates specialised reasoning across startup strategy, market research, narrative development and validation before producing structured founder outputs.

> **Note**
>
> This repository presents the public architecture only.
> Proprietary prompts, reasoning logic, production infrastructure and commercial implementations are not included.

---

# System Overview

```text
                     Founder
                        │
                        ▼
               Founder Interface
                  (Streamlit UI)
                        │
                        ▼
                 FastAPI Backend
                        │
 ┌──────────────┬──────────────┬──────────────┐
 ▼              ▼              ▼
Input      Reasoning      Validation
Pipeline      Engine         Engine
 └──────────────┬──────────────┘
                ▼
        Strategic Synthesis
                │
                ▼
        Founder Reports
        Investor Memo
   Strategic Recommendations
```

---

# AI Architecture

| Layer | Purpose |
|--------|---------|
| Founder Interface | Collects and structures founder input |
| Input Pipeline | Normalises and prepares information for reasoning |
| Reasoning Engine | Coordinates specialised AI reasoning across strategy, research and narrative |
| Validation Engine | Scores evidence, consistency and execution readiness |
| Strategic Synthesis | Combines specialised outputs into one coherent recommendation |
| Output Layer | Produces structured founder reports and strategic recommendations |

---

# Core Reasoning Modules

| Module | Responsibility |
|--------|----------------|
| Category Inference | Startup classification |
| Research | Market and competitor analysis |
| Strategy | Business model, GTM and positioning |
| Narrative | Founder story and investor messaging |
| Strategic Synthesis | Combines all reasoning outputs |
| Validation | Consistency and quality assessment |
| Rubric Scoring | Investment readiness evaluation |
| Traction Analysis | Evidence maturity assessment |
| Investor Challenges | Strategic stress-testing |
| Slide Planning | Structured presentation planning |

---

# Engineering Principles

| Principle | Description |
|-----------|-------------|
| Modular | Independent reasoning components designed for scalability |
| Explainable | Structured reasoning rather than opaque generation |
| Deterministic | Schema-driven outputs where appropriate |
| Extensible | New reasoning modules can be added independently |
| AI-Native | Designed around coordinated AI reasoning rather than single-prompt generation |

---

# Technology Stack

| Layer | Technology |
|--------|------------|
| Language | Python 3.11 |
| Backend | FastAPI |
| Founder Interface | Streamlit |
| Data Models | Pydantic |
| Contracts | JSON Schema |
| Presentation | python-pptx |
| APIs | REST |
| Development | GitHub Codespaces |
| AI Development | Devin • OpenAI Codex |

---

# Repository Scope

| Included | Not Included |
|----------|--------------|
| Multi-agent architecture | Proprietary prompts |
| Engineering approach | Production reasoning logic |
| Public documentation | Commercial implementations |
| Technology stack | Internal infrastructure |
| System architecture | Customer projects |

---

© Pitch Agent
