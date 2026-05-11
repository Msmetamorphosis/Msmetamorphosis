<h1 align="center">👋 Hi, I'm Crystal Tubbs</h1>
<h3 align="center">AI Systems Researcher & Builder | MSAI Candidate | AI x Blockchain Strategist | Founder, Metamorphic Curations</h3>

## About

I build AI systems that make accountability and equity more than buzzwords. My work sits at the intersection of applied AI research, governance, and real-world deployment, driven by the belief that technology should contribute to a more equitable world, not widen existing gaps.

## Background

Former military brat. Serial entrepreneur with 20+ years building businesses across e-commerce and service industries. I entered AI in my late 30s, earned a 4.0 GPA in my MSAI program at Kennesaw State University (graduating July 2026), and built a research portfolio that bridges theory and practice.

My path has never been conventional, and that is the point. Perspective earned through lived experience shapes everything I build.

---

# What I Build

## ALETHEIA Protocol

A two-layer discretionary mutual protection protocol for the agentic economy. Built at the EasyA x CoinDesk Consensus Miami Hackathon 2026.

Layer 1 is an Agent Risk Registry where developers register AI agents on-chain, declare financial boundaries and system prompt hashes, and receive a Claude-evaluated composite risk score across eight dimensions.

Layer 2 is a Mutual Protection Pool where registered agents become coverable, members pay risk-adjusted USDC contributions via x402 on Base, and spend cap breaches are verified mathematically from on-chain data with no user testimony required. Claude on Amazon Bedrock arbitrates claims and the pool pays automatically.

### Key Features

- On-chain agent identity registry
- Cryptographic spend cap verification
- Claude-based multidimensional risk scoring
- x402 USDC contribution infrastructure
- Autonomous claim adjudication
- Planned integration with CHRYSALIS governance architecture

**Live:** https://aletheiaprotocol.io/  
**Repo:** https://github.com/Msmetamorphosis/aletheia-protocol

---

## CHRYSALIS

An epistemic governance framework for agentic AI.

Rather than allowing agents to self-govern, CHRYSALIS validates agent beliefs before action through external accountability mechanisms. The framework focuses on epistemic integrity, belief validation, adversarial resistance, and governance transparency for autonomous systems.

### Core Modules

- **MEMOIR** -- Belief classification and on-chain attestation to Solana
- **ORACLE** -- Metacognitive feedback and reflective reasoning loop
- **MIRROR** -- Real-time cognitive state monitoring
- **COMPASS** -- Regulatory compliance and audit reporting
- **SHIELD** -- Adversarial belief injection detection
- **EIS** -- Agent reputation and trust scoring

### Key Capabilities

- Externalized agent governance
- Real-time epistemic integrity scoring
- Cognitive state monitoring
- On-chain governance attestations
- AI accountability infrastructure
- Adversarial belief defense systems

**Live:** https://chrysalisai.io  
**Dashboard:** https://chrysalis-omega.vercel.app

---
## LLM Reliability Pipeline

A full-stack AI research dashboard testing whether a minimal reliability layer reduces LLM output failures across behavioral prompt variations.

The project compares three systems across four prompt styles to evaluate whether failures come from model capability or from the way users phrase prompts in real-world enterprise environments.

### Systems Tested

| System | Description | LLM Calls Per Output |
|---|---|---:|
| Baseline A | Direct LLM, no retrieval, no validation | 1 |
| Baseline B | ChromaDB retrieval, no validation | 1 |
| Pipeline | RAG + self-critique + schema validation + repair | 2 to 3 |

### Prompt Styles Tested

- **Structured:** explicit, well-formed, professional
- **Ambiguous:** underspecified and vague
- **Verbose:** over-explained with the request buried
- **Casual:** informal, typo-prone, conversational

### Results

| System | Structured | Ambiguous | Verbose | Casual |
|---|---:|---:|---:|---:|
| Baseline A | 100% | 0% | 0% | 0% |
| Baseline B | 100% | 0% | 0% | 0% |
| Pipeline | 100% | 100% | 100% | 100% |

Key Findings:  1. Prompt style can determine output quality more than model capability. Baseline A showed a 100 percentage point compliance gap between structured and casual prompts despite a 100% JSON parse rate, demonstrating how production systems can silently fail even when outputs appear technically valid. 2. Prompt style can degrade model output, but architectural stabilization is possible.

The LLM Reliability Pipeline showed that baseline systems failed under ambiguous, verbose, and casual prompt styles, while the pipeline achieved 100% schema compliance across all prompt styles by adding a minimal reliability layer:  one self-critique pass, schema validation, and repair.

This means varied user prompt behavior does not have to result in production failure. A lightweight stabilization architecture can preserve compliance even when prompt quality varies.

### Domain and Metrics

- **Domain:** VA veteran benefits
- **Model:** Claude via Anthropic API
- **Metrics:** JSON schema compliance, field accuracy against ground truth, output variance, and latency
- **Data:** 15 extraction samples, 25 QA pairs with ground truth, and 20 VA benefits passages for retrieval

**Repo:** https://github.com/Msmetamorphosis/llm-reliability-dashboard
**Live:** https://msmetamorphosis.github.io/llm-reliability-dashboard

---

## CRAFT

### Contextual Rewriting and Fidelity Tester

CRAFT is a prompt quality analysis and improvement tool built from the findings of the LLM Reliability Pipeline project.

The Reliability Pipeline demonstrated that prompt style strongly affects output quality, schema compliance, and production reliability. CRAFT operationalizes that research into a practical enterprise tool that diagnoses prompts, scores them against task-appropriate rubrics, rewrites them with fidelity to the original intent, and shows measurable improvement in output quality.

### What CRAFT Does

- Classifies a prompt into one of five enterprise task types
- Scores the prompt against a task-appropriate rubric from 0 to 100
- Runs the original prompt through Claude and scores the output
- Rewrites the prompt by fixing automated gaps and flagging user-only gaps with placeholders
- Runs the improved prompt and scores the new output
- Shows a side-by-side comparison with quantified improvement

### Five Task Types

| Type | Description | Example |
|---|---|---|
| Extraction | Pulling structured data from text | Extract fields from a contract |
| Reasoning | Analyzing situations and applying rules | Does this employee qualify for FMLA? |
| Generation | Drafting content and communications | Write an email to a client |
| Ideation | Brainstorming and creative exploration | Ideas for a new product feature |
| Conversational | Guidance, coaching, and policy questions | How do I handle this situation? |

### Scoring

**Prompt Quality Score:** A 0 to 100 rubric-based audit of the prompt against task-appropriate criteria, including clarity of intent, context completeness, specificity, and output specification. Rubric weights shift by task type.

**Output Quality Score:** A 0 to 100 Claude-evaluated assessment of the actual output against task-appropriate dimensions, such as schema compliance for extraction, actionability for reasoning, and tone fit for generation.

**Ceiling Score:** The maximum score achievable with the information provided. Some gaps can only be filled by the user, and CRAFT identifies those gaps directly.

### Research Context

CRAFT extends the LLM Reliability Pipeline research by investigating whether prompt-level interventions, specifically completeness auditing and task-appropriate rewriting, improve output quality across enterprise task types.

The hypothesis is that improvement will be largest for reasoning and conversational tasks, which are often the most underspecified in practice.

**Live:** https://msmetamorphosis.github.io/CRAFT/  
**Related Project:** https://github.com/Msmetamorphosis/llm-reliability-dashboard
---

## VetNavi

A retrieval-augmented generation (RAG) platform designed to support veteran career transitions and workforce reintegration.

Built as my MSAI capstone project, VetNavi combines semantic retrieval, personalized AI guidance, and contextual career translation systems to help veterans navigate the difficult transition from military to civilian employment.

The platform focuses on reducing systemic friction by helping veterans:
- Translate military experience into civilian job language
- Identify aligned career pathways
- Navigate education and certification opportunities
- Discover relevant benefits and transition resources
- Receive personalized career guidance through AI-assisted interaction

VetNavi was designed with an emphasis on accessibility, equity, and practical real-world usability for underserved communities often overlooked by traditional hiring systems.

**Live:** https://vetnavi.ai
---

# Production AI Systems

## AI Financial Intelligence Agent

Built a fully automated financial intelligence system for business operations, revenue analysis, and tax tracking.

The system transformed operational decision-making by allowing business owners to query financial performance in natural language, including:
- Revenue trend analysis
- Store performance comparisons
- Operational shift analysis
- Staffing optimization
- Inventory forecasting
- Re-engagement campaign targeting

### Technologies and Focus Areas

- Agentic AI
- Financial intelligence systems
- NLP interfaces
- Business analytics automation

---

## Logistics Fleet Web Application + Agent Integration

Designed and built a logistics web platform with integrated agentic capabilities for fleet management and operational automation.

The platform replaced manual dispatching, compliance recordkeeping, and operational reporting with scalable AI-assisted automation.

### Capabilities

- Fleet operations management
- Intelligent dispatch workflows
- Automated compliance tracking
- Operational reporting automation
- Agent-assisted logistics coordination

---

## Franchise Operations Automation Suite

Built multi-agent operational systems for franchise organizations that automate recordkeeping, surface performance insights, identify declining markets, and recommend targeted campaign strategies.

### System Features

- Multi-agent coordination
- Franchise performance analytics
- Market decline detection
- Campaign strategy recommendation
- Cross-location operational visibility

---

## Custom Prompt Libraries Across Industries

Designed and delivered custom prompt engineering libraries tailored to organization-specific workflows and objectives.

Industries supported include:
- Legal offices
- Beauty salons
- Logistics companies
- Restaurants
- C-suite executive operations

Each library was built around operational context, workflow optimization, and domain-specific AI interaction patterns rather than generic prompting templates.

---

## Automated Trading and Digital Asset Agents

Built automated trading agents and multi-platform digital asset intelligence systems focused on portfolio tracking, tax optimization, and financial analytics.

### Capabilities

- Automated trading workflows
- Cost basis tracking across exchanges
- Tax strategy automation
- DeFi portfolio aggregation
- Blockchain analytics and reporting

---

# Research

### CIPHER Covert Influence Passed via Hidden Encoding in Representations : Evaluating Subliminal Bias Transfer During Knowledge Distillation
Covert bias transfer via knowledge distillation. Introduced the concept of **Metric Illusion**.
http://digitalcommons.kennesaw.edu/cday/Fall_2025/Masters_Research/16
https://digitalcommons.kennesaw.edu/cgi/viewcontent.cgi?article=1647&context=cday

### PRISM Proxy Recognition and Inclusion Scoring Method
Published in Symposium of Student Sccholars @ KSU Commons, Presented at KSU CCSE Computing Showcase, Fall 2025 (Graduate Research)

Research on context-dependent bias in LLM resume screening.
http://digitalcommons.kennesaw.edu/undergradsymposiumksu/fall2025/fall2025/28
https://digitalcommons.kennesaw.edu/cgi/viewcontent.cgi?article=4639&context=undergradsymposiumksu


### SAF
Surrogate Accountability Framework for agentic AI governance. **2nd place Graduate Capstone winner at KSU CCSE Computing Showcase Spring 2026.**
https://digitalcommons.kennesaw.edu/cgi/viewcontent.cgi?article=1731&context=cday
https://digitalcommons.kennesaw.edu/cday/Spring_2026/Graduate_Project/12/


### Mitigating Prompt-Induced Variability in LLM Outputs

https://digitalcommons.kennesaw.edu/cday/Spring_2026/Masters_Research/17/
https://digitalcommons.kennesaw.edu/cgi/viewcontent.cgi?article=1752&context=cday

### From Leakage to Reliability in Dementia Detection

https://digitalcommons.kennesaw.edu/cday/Spring_2026/Masters_Research/18/
https://digitalcommons.kennesaw.edu/cgi/viewcontent.cgi?article=1753&context=cday
---

# Hackathon

## EasyA x CoinDesk Consensus Miami 2026

Built ALETHEIA Protocol as a solo technical founder with financial modeling by Esteban Cerda Le - Bert (Protocol Financial Strategist).

ALETHEIA is a discretionary mutual protection protocol covering cryptographically verifiable AI agent financial failures on Base Sepolia.

### Features

- Agent identity registry
- Claude-based risk scoring
- x402 USDC contribution infrastructure
- Mathematical breach verification
- Autonomous claims arbitration

### Q3 2026 Roadmap

Integration with CHRYSALIS epistemic governance on Solana, enabling governed agents to receive up to a 50% reduction in contribution costs based on verified governance integrity.

---

# Philosophy

I build technology that serves people who have historically been underserved by it.

Equity in AI is not a feature request. It is a design requirement.

Every framework, system, and line of research I produce is measured against a simple question:

> Does this move us closer to a world where powerful technology works for everyone?

---

# Connect

**Consultancy:** Metamorphic Curations LLC  
https://www.metamorphiccurations.com/

Make it a great day.
