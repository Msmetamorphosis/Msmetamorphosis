<h1 align="center">👋 Hi, I'm Crystal Tubbs</h1>
<h3 align="center">AI Systems Researcher & Builder | MSAI Candidate | AI x Blockchain Strategist</h3>


I design and build AI systems that work in the real world — from agentic pipelines and enterprise tooling to published research on LLM behavioral stability, bias propagation, and AI governance. I'm finishing my Master's in AI at Kennesaw State University (4.0 GPA, expected Summer 2026) while running Metamorphic Curations LLC, an AI transformation consultancy.

My work sits at the intersection of rigorous engineering and responsible deployment: building things that are technically sound, ethically considered, and actually useful to the humans using them. My personal mission is to use technology as a tool for conscious equity; designing systems that don't just perform well, but expand access, reduce harm, and build a more just world.

---

## Research

My published and in-progress research centers on LLM behavior, fairness, and accountability. Papers presented at **KSU Computing Day** and the **KSU Symposium of Student Scholars**, both Fall 2025.

**[CIPHER](https://msmetamorphosis.github.io/Project-CIPHER/)** — *Covert Influence Passed via Hidden Encoding in Representations Evaluating Subliminal Bias Transfer During Knowledge Distillation*
Identified a covert bias injection mechanism using Unicode signals and column order shifts that evades standard fairness audits (SPD/EOD metrics). Reframed as label-mediated bias propagation invisible to conventional evaluation pipelines. **47 downloads** on KSU Digital Commons. Advised by Dr. Martin Brown. Presented at KSU C-Day Fall 2025. · [KSU Repository](https://digitalcommons.kennesaw.edu/cday/Fall_2025/Masters_Research/16/)

**[PRISM](https://digitalcommons.kennesaw.edu/cday/Fall_2025/Masters_Research/14/)** — *Proxy Recognition and Inclusion Scoring Method: Evaluating Context-Dependent Bias in Large Language Models for Resume Screening*
Co-authored study on how subtle demographic signals embedded in first names influence AI resume screening, even when candidate qualifications are identical. Tested across a controlled dataset of 324 synthetic resumes against GPT-3.5 and Sentence-BERT across technology, healthcare, and law job postings. **22 downloads** on KSU Digital Commons + **16 downloads** via KSU Symposium of Student Scholars. Includes a [recorded presentation](https://digitalcommons.kennesaw.edu/undergradsymposiumksu/fall2025/fall2025/28/). Co-authored with Destiny Raburnel.

**BRIDGE** — *Blockchain Receipt Intelligence for Developing Greater Equity: Tokenizing Financial Inclusion Through Computer Vision-Based Receipt Verification* · [Poster](https://msmetamorphosis.github.io/Project-CIPHER/bridge-poster.jpg)
Computer vision pipeline that extracts financial data from photographed receipts, evaluates recurring payment patterns, and anchors verified records on a blockchain ledger to build portable, tokenized credit histories for underbanked populations. Combines OCR preprocessing, Form Recognizer document intelligence, and prototype credit scoring anchored on Polygon. **Active/ongoing study, Spring 2026.** Advised by Dr. Sanghoon Lee.

**SAF** — *Surrogate Accountability Framework* 
Proposed an entitlement-based governance model for agentic AI systems, incorporating continuous observability and lifecycle accountability. Addresses the gap between current AI policy and the operational reality of autonomous agents. Developed as my project for the AI Ethics course under Dr. Martin Brown, KSU MSAI program.

**UIBF** — *User-Induced Behavioral Fields*
Theoretical framework exploring how persistent user interaction patterns shape emergent LLM behavior at the session and system level.

**LLM Behavioral Stability Under Prompt Variation** *(Big Data Analytics — Course Project)*
Empirically validated that a generate → critique → validate+repair pipeline achieves 100% schema compliance across all prompt styles at 2x LLM call cost. Confirmed architectural path to behavioral stability without fine-tuning. Completed as part of the Big Data Analytics course under Dr. Martin Brown, KSU MSAI program.

---

## Featured Projects
**[VetNavi.ai](https://vetnavi.ai/) — NextMission Navigator** · [GitHub](https://github.com/Msmetamorphosis/NextMission-VetNavi-v2)
Full-stack AI platform built to help veterans navigate post-service transitions. Uses RAG, Claude API, Zod schema validation, and structured agent reasoning to surface personalized benefit and career pathways. Currently being rebuilt and enhanced as my MSAI capstone project under Dr. Arthur Choi.
`Next.js 14 · React · TypeScript · Tailwind CSS · Claude API · RAG · Zod · Vercel · Full-Stack`

**[CRAFT](https://msmetamorphosis.github.io/CRAFT/) — Contextual Rewriting and Fidelity Tester**
Enterprise prompt coaching product under Metamorphic Curations. FastAPI/SSE backend deployed on Render, GitHub Pages frontend. Helps teams diagnose and repair prompt drift, schema failures, and LLM behavioral inconsistency.
`Python · FastAPI · SSE · Claude API · JSON Schema · Render · GitHub Pages`

**[LLM Reliability Pipeline](https://msmetamorphosis.github.io/llm-reliability-dashboard/)** · [GitHub](https://github.com/Msmetamorphosis/llm-reliability-dashboard)
Experimental pipeline testing whether a self-critique and validation layer improves LLM schema compliance and output quality across varied prompt styles. Achieved 100% schema compliance — findings directly inform the Big Data Analytics course project research.
`Python · FastAPI · Uvicorn · Anthropic API · ChromaDB · Pydantic · JSON Schema · SSE · Render · GitHub Pages`

**DementiaNet** · [GitHub](https://github.com/Msmetamorphosis/NeuralNets_Project_DementiaNet)
Neural network project using Wav2Vec2 and SpecAugment for dementia detection from speech. Co-authored with Destiny Raburnel as part of the Neural Networks and Deep Learning course under Dr. Zongxing Xie, KSU MSAI program.
`Python · PyTorch · Wav2Vec2 · SpecAugment · HuggingFace Transformers · librosa · torchaudio · scikit-learn · Speech Processing`

**Legal Practice Dual-Agent System**
Document generation and legal research dual-agent architecture for a small law firm. Handles structured document output with agent handoff and validation checkpoints. *Built under NDA — code and client details confidential.*
`Python · LangChain · RAG · Claude API · Document Generation · Agentic AI`

**Financial Automation Agent**
Conversational RAG interface with Square/POS/banking integrations for a small business client. Reconstructed three years of financial records and delivered an interactive query layer over structured financial data. *Built under NDA — code and client details confidential.*
`Python · OpenAI API · RAG · Square API · Zapier · Google Sheets · SQLite · Conversational AI`

**Crypto Cost Basis Reconciliation Tool**
Fuzzy matching and transaction graph analysis tool for reconciling multi-exchange cryptocurrency portfolios. Handles messy, incomplete transaction histories and outputs audit-ready cost basis reports.
`Python · RapidFuzz · NetworkX · Pandas · Graph Analysis · Financial Engineering`

---

## AI x Blockchain

I've been at the intersection of AI and decentralized systems since before it was a conference track. I'm currently developing an **AI x blockchain product** being presented at **Consensus 2026**, and my BRIDGE research project is an active application of this — using computer vision, OCR, and Polygon-anchored verification to build portable credit identities for underbanked populations.

My background here includes protocol and whitepaper analysis, on-chain data modeling, portfolio strategy, and building autonomous trading systems. I believe the convergence of AI agents and decentralized infrastructure is one of the most important architectural frontiers of the next decade, and I'm building in it.

---

## LLM Training Contributions

Through contracted roles on programming and data science teams — including work under NDA with major AI labs — I've contributed directly to frontier LLM development across instruction tuning, code evaluation, mathematical reasoning, and preference ranking. This work required deep familiarity with model behavior, failure modes, and the gap between what models produce and what humans actually need.

---

## Earlier Work

The projects that got me here: custom GPT agents, prompt engineering pipelines, fine-tuning experiments on GPT-3.5 Turbo, SQL training data curation, custom datasets for LLM evaluation, and Python prompt/unit test suites for model training. The foundations matter.

Web development roots: **The Goldstein Law Firm** and **Metamorphic Curations LLC** — both designed and built by yours truly.

---

## Currently

- Finishing MSAI at KSU | Graduating summer 2026
- Deploying CRAFT under Metamorphic Curations
- Preparing papers for KSU Computing Day
- Prepping MEMOIR Chain, an AI x blockchain product for presentation at Consensus 2026
- Open to full-time roles in AI transformation, enablement, architecture, and engineering

---

## Let's Connect

If you're building something at the frontier of AI systems, responsible deployment, or AI x blockchain, I'd  love to hear about it.

[Email](mailto:msmetamorphosis@metamorphiccurations.com) · [LinkedIn](https://www.linkedin.com/in/crystal-tubbs/) · [Metamorphic Curations](https://www.metamorphiccurations.com)

---

<h3 align="center">✨ Make it a GREAT day!</h3>

