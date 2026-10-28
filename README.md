<div align="center">

# Orvyen
### Autonomous AI Agent Security & Regulatory Compliance

[![Orvyen Agentic](https://img.shields.io/badge/Orvyen_Agentic-v0.3.0-blue?logo=shield)](https://github.com/orvyen/orvyen-agentic)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Singapore IMDA](https://img.shields.io/badge/Singapore-IMDA_Agentic_AI_(May_2026)-green)](https://www.imda.gov.sg/)
[![OWASP LLM Top 10](https://img.shields.io/badge/OWASP-LLM_Top_10-orange)](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

---

> **Pre-deployment static analysis security and compliance scanning for modern AI agent architectures.**  
> *LangChain &bull; LangGraph &bull; CrewAI &bull; Model Context Protocol (MCP)*

</div>

<br/>

## 🎯 About Orvyen

While 76% of existing AI security solutions operate at runtime (inspecting prompts downstream after deployment), **Orvyen** operates **pre-deployment in CI/CD and local development** — finding security flaws in agent code, prompt templates, tool privileges, and MCP server manifests before code ever merges.

---

## 🚀 Flagship Project: [Orvyen Agentic](https://github.com/orvyen/orvyen-agentic)

A CLI-first static analysis engine purpose-built for modern AI agent graphs:

- **Agent-Aware AST Parsing**: Deep inspection of Python agent graphs and multi-agent orchestrations across **LangChain**, **LangGraph**, and **CrewAI**.
- **Model Context Protocol (MCP) Scanning**: Static inspection of `claude_desktop_config.json` and `mcp.json` server configurations, detecting shell capabilities, plaintext credentials, and orphaned gateways.
- **Sub-10ms Performance**: Zero external runtime dependencies; executes blazing-fast static checks in milliseconds using Python's standard library.
- **Agent Bill of Materials (AIBOM)**: Auto-compiles an auditable inventory of every tool, privilege tier (`READ`, `WRITE`, `EXECUTE`, `ADMIN`), model, and external data flow.
- **Regulatory & Governance Scorecards**:
  - **Singapore IMDA**: Model AI Governance Framework for Agentic AI (May 2026 v1.5 - 4 Pillars).
  - **MAS Guidelines**: Monetary Authority of Singapore AI Risk Management Guidelines.
  - **OWASP LLM Top 10**: Direct vulnerability mapping to the official standard.

---

## 📦 Quick Installation

```bash
# Python
pip install orvyen-agentic

# Node.js
npm install -g orvyen-agentic
```

### Basic Scan
```bash
orvyen-agentic scan .
```

---

<div align="center">
  <sub>Developed by <b>Algorzen Pte. Ltd.</b> (Singapore) &bull; Official Repository: <a href="https://github.com/orvyen/orvyen-agentic">orvyen/orvyen-agentic</a></sub>
</div>
