# Enterprise AI Hub Architecture

Architecture blueprint for building a unified AI-powered chat interface that connects all enterprise systems — using **Claude** as the orchestration engine.

## Overview

This repository contains the technical architecture for an **Enterprise AI Hub**: a single natural-language interface where employees can query and act on information from Salesforce, Jira, Confluence, SAP, Workday, GitHub, and any other system — without switching tools.

Claude (Anthropic) acts as the central brain: it interprets questions, calls the right systems via tool use, and synthesises answers.

## 📖 Architecture Document

➡️ **[Read the full architecture: `docs/architecture.md`](docs/architecture.md)**

## Table of Contents

| # | Section |
|---|---|
| 1 | [Core Philosophy](docs/architecture.md#1-core-philosophy) |
| 2 | [Claude as the Central Brain](docs/architecture.md#2-claude-as-the-central-brain) |
| 3 | [Three Integration Strategies](docs/architecture.md#3-three-integration-strategies) |
| 4 | [Security & Governance](docs/architecture.md#4-security--governance) |
| 5 | [Enterprise Knowledge Layer (RAG)](docs/architecture.md#5-enterprise-knowledge-layer-rag) |
| 6 | [Automation Engine](docs/architecture.md#6-automation-engine) |
| 7 | [Multi-Agent Evolution](docs/architecture.md#7-multi-agent-evolution) |
| 8 | [Observability & Continuous Improvement](docs/architecture.md#8-observability--continuous-improvement) |
| 9 | [Decision Matrix](docs/architecture.md#9-decision-matrix) |
| 10 | [Complete Architecture Diagram](docs/architecture.md#10-complete-architecture-diagram) |
| 11 | [Team Structure](docs/architecture.md#11-team-structure) |
| 12 | [Technology Stack Summary](docs/architecture.md#12-technology-stack-summary) |
| 13 | [Getting Started — First 30 Days](docs/architecture.md#13-getting-started--first-30-days) |
| 14 | [Phased Roadmap](docs/architecture.md#14-phased-roadmap) |

## Three Integration Strategies

The hub supports three complementary strategies for connecting Claude to enterprise systems:

| Strategy | Mechanism | Best For |
|---|---|---|
| **A — Direct API Integration** | Claude calls system APIs (REST, OData, SQL) via tool use | Write access, sensitive data, no MCP available |
| **B — MCP Servers** | Claude connects via Model Context Protocol | Standard read/search patterns, growing ecosystem |
| **C — Native AI in Business Systems** | Salesforce Einstein, Atlassian Intelligence, ServiceNow AI handle domain tasks; Claude synthesises | Domain-specialised AI from best-of-breed vendors |

## Repository Structure

```
README.md          — Project overview and links
docs/
  architecture.md  — Full architecture document
```
