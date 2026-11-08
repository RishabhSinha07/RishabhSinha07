### Hi, I'm Rishabh 👋

## AI Engineer · Agent Systems · LLM Tooling · Full-Stack

I build **production AI systems** — autonomous agents, MCP tooling, RAG pipelines, and browser-native ML. Most of what's below is a working system with a live demo, not a notebook: multi-agent orchestration on **LangGraph** and **Bedrock**, vector search on **pgvector**, transformer inference compiled to **WebAssembly**, and serverless pipelines on **AWS Lambda**.

I also build the layer underneath — autograd engines and language models written from scratch, no frameworks — because knowing what the abstraction is doing is the difference between using a model and engineering with one.

---

## 🤖 Agents & AI Infrastructure

<table>
<tr>
<td width="50%">

### ⭐ [Scribe](https://github.com/RishabhSinha07/AgentHarnessToScribe)
**A whiteboard an agent can draw on while it teaches.**

Mermaid and SVG describe a *finished* picture — neither can erase, and neither can point. Scribe is a stateful canvas, a small drawing language, and an **MCP server** so any LLM can draw live, narrate as it goes, gesture at what it means, and rub out what it got wrong.

**[▶ Watch it draw itself](https://rishabhsinha07.github.io/AgentHarnessToScribe/)** — a lesson replayed stroke by stroke, narrated aloud.

`Python` `MCP` `Model Context Protocol` `Canvas` `uv` `pytest`

</td>
<td width="50%">

### [CurateAI](https://github.com/RishabhSinha07/CurateAI)
**Multi-agent consultation system for personalized product recommendations.**

Identifies a user's problem, personalizes through clarifying questions, then recommends via semantic search guided by a knowledge graph. Agent orchestration is a **LangGraph state machine** over an async FastAPI core, with `pgvector` for retrieval and `NetworkX` for graph reasoning.

**[▶ Demo video](https://youtu.be/svhhO4ivPEc)**

`LangGraph` `AWS Bedrock` `Nova Pro` `FastAPI` `PostgreSQL + pgvector` `Docker`

</td>
</tr>
<tr>
<td width="50%">

### [ReelForge](https://github.com/RishabhSinha07/ReelForge)
**One idea → a finished Instagram Reel, fully automated.**

Orchestrates specialized agents across the whole media pipeline: structured planning, cinematic scripting with **Claude 3.5 Sonnet**, vertical image generation via **Nova Canvas**, neural voice-over with **Polly**, then assembly into a synced 1080×1920 MP4 with cross-fades.

`Python` `Claude 3.5 Sonnet` `Amazon Bedrock` `Nova Canvas` `Polly` `MoviePy`

</td>
<td width="50%">

### [EpicToSprintPlanner](https://github.com/RishabhSinha07/EpicToSprintPlanner)
**1000+ page documents → INVEST-compliant sprint backlogs.**

A serverless fan-out pipeline — chunker → story generator → aggregator — that produces user stories with acceptance criteria, story-point estimates, and dependency mapping, exported as Jira-ready JSON. Defined as infrastructure-as-code with SAM.

`AWS Lambda` `Bedrock` `SAM` `S3` `Serverless` `Python`

</td>
</tr>
<tr>
<td width="50%">

### [Morning Ops Agent](https://github.com/RishabhSinha07/morning-ops-agent)
**A daily operations briefing for your commute.**

Fetches live weather and local news for any city, reasons over both with an LLM to surface transit disruptions, closures and alerts, then publishes a readable briefing to **Notion**. Ships on a **GitHub Actions** schedule and runs unattended every day.

`Python` `LLM Agents` `Notion API` `GitHub Actions` `uv`

</td>
<td width="50%">

### [agenticDev](https://github.com/RishabhSinha07/agenticDev)
**A 4-agent development pipeline for solo devs.**

PM Spec → Architect Review → Implementation → Code Review, taking a feature idea through to reviewed code. An agent-definition harness rather than an application — the prompts and role boundaries *are* the artifact.

`Claude Code Agents` `Agent Design`

</td>
</tr>
</table>

---

## 🧠 Applied ML & Models From Scratch

<table>
<tr>
<td width="50%">

### [RedactAI](https://github.com/RishabhSinha07/redactai)
**PII redaction where the document never leaves your machine.**

A **BERT NER model runs entirely in the browser** via ONNX/WebAssembly, in a Web Worker so the UI never blocks. Combines regex matching with ML entity recognition to catch SSNs, names and organizations. Zero uploads is an architectural guarantee, not a policy promise. E2E tested with Playwright.

**[▶ Live demo](https://redactai-beige.vercel.app)**

`Transformers.js` `ONNX / WASM` `BERT NER` `React` `PDF.js` `Playwright`

</td>
<td width="50%">

### [Neural Networks Playground](https://github.com/RishabhSinha07/NeuralNetworks-Playground)
**An autograd engine built from first principles.**

A `Tensor` with real reverse-mode `.backward()`, a scalar MLP, then the same network rebuilt as a **batched matrix engine** with Xavier init and trained on a real dataset. Framework-free, following Karpathy's micrograd and extended well past it.

`Python` `Autograd` `Backpropagation` `NumPy`

</td>
</tr>
<tr>
<td width="50%">

### [Neural Network from Scratch](https://github.com/RishabhSinha07/NN)
Built by hand in Python and NumPy — no ML frameworks. A 20-step roadmap from a 2-input toy problem up to CIFAR-10, with per-step derivations and visualizations kept strictly separate from the implementation.

`Python` `NumPy` `Deep Learning`

</td>
<td width="50%">

### [Makemore](https://github.com/RishabhSinha07/Makemore)
Character-level language models built up layer by layer — bigram counts, then an MLP — following Karpathy's makemore series.

`PyTorch` `Language Models` `Jupyter`

</td>
</tr>
</table>

---

## 🛠️ Developer Tools & Full-Stack

<table>
<tr>
<td width="50%">

### [Automated API Testing](https://github.com/RishabhSinha07/Automated-API-Testing)
Generates and *maintains* API test suites from OpenAPI specs. A deterministic IR parser normalizes OpenAPI 3.x, smart diffing detects added/updated/deleted endpoints **while preserving hand-written test code**, and a mutation engine auto-generates negative cases for missing fields, wrong types and boundary violations.

`Python` `OpenAPI` `Test Generation` `CLI`

</td>
<td width="50%">

### [CurateAI Widget](https://github.com/RishabhSinha07/curateai-widget)
An embeddable AI chat widget that drops into any site with a single script tag. **Shadow DOM** isolation so it can't collide with host styles, plus product carousels, suggested replies and a login flow — all in a lightweight Preact bundle.

**[▶ Live demo](https://curateai-widget.vercel.app)**

`TypeScript` `Preact` `Shadow DOM` `Vite`

</td>
</tr>
<tr>
<td width="50%">

### [KG Explorer](https://github.com/RishabhSinha07/kg-explorer)
Import any JSON or YAML knowledge graph, visualize nodes and relationships, and edit the whole thing with drag-and-drop.

**[▶ Live demo](https://kg-explorer-umber.vercel.app)**

`TypeScript` `Graph Visualization`

</td>
<td width="50%">

### [ResumeCraft](https://github.com/RishabhSinha07/ResumeCraft)
ATS-friendly resume builder — three templates, real-time preview, drag-and-drop reordering, instant template switching and pixel-perfect PDF export.

**[▶ Live demo](https://resume-craft-indol.vercel.app)**

`TypeScript` `React` `Tailwind` `Framer Motion`

</td>
</tr>
<tr>
<td width="50%">

### [Crisis Resource Map](https://github.com/RishabhSinha07/crisis-resource-map)
Interactive map for finding and sharing emergency resources in conflict zones — connecting people to critical supplies and services when it matters most.

**[▶ Live demo](https://crisis-resource-map.vercel.app)**

`Next.js` `TypeScript` `Mapping`

</td>
<td width="50%">

### Algorithm Visualizers
[**Sorting**](https://rishabhsinha07.github.io/SortingAlgorithmsVizz/) — side-by-side sorting algorithm races.
[**Shortest Path**](https://rishabhsinha07.github.io/ShortestPathVisualization/) — interactive pathfinding on a grid.

`JavaScript` `Algorithms`

</td>
</tr>
</table>

---

## 🧰 Tech Stack

**AI / ML** — LangGraph · LangChain · Amazon Bedrock (Claude, Nova Pro, Nova Canvas) · OpenAI · HuggingFace · Transformers.js · ONNX Runtime · PyTorch · NumPy
**AI Patterns** — Multi-agent orchestration · MCP servers · RAG · Tool calling · Vector search · Knowledge graphs · NER · Prompt engineering · On-device inference
**Backend** — Python · FastAPI · Node.js · PostgreSQL + pgvector · AWS Lambda · SAM · Docker
**Frontend** — React · Next.js · TypeScript · Preact · Tailwind · Vite
**Practice** — uv / pyproject · pytest · Playwright E2E · GitHub Actions CI · Infrastructure-as-code

---

## 🤝 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishabh-sinha-99a706164/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://portfolio-two-pink-14.vercel.app)
