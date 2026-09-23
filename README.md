# Orvyen Agentic

**Status: In Active Development**

Static security and compliance scanning for AI agent architectures.

Orvyen Agentic is a CLI-first static analysis engine purpose-built for AI agents. It parses agent code and configuration to identify security vulnerabilities and compliance risks before deployment, supporting LangChain, LangGraph, CrewAI, and Model Context Protocol (MCP) deployments.

## Capabilities

* **Tool Permission Scoping:** Detects tools granted broader access than their declared purpose requires.


* **Injection Surface Detection:** Identifies unsanitized input concatenated directly into system prompts.


* **Secret Scanning:** Locates API keys and credentials committed into agent configuration files.


* **Data Flow Tracing:** Tracks personal data flowing into third-party tool calls or logs without a redaction step.


* **Recursion Bounds:** Identifies agent-to-agent delegation lacking depth or cost circuit breakers.


* **Infrastructure Auditing:** Flags orphaned tools and MCP servers wired in but no longer referenced.


* **Compliance Reporting:** Automatically generates an Agent Bill of Materials (AIBOM) mapped to the OWASP LLM Top 10 and Singapore's IMDA/MAS governance frameworks.



## Installation (Coming Soon)

Packages for both Python and Node.js environments are currently in production and will be published shortly.

**Python:**

```bash
# pip install orvyen-agentic

```

**npm:**

```bash
# npm install -g orvyen-agentic

```

## Usage (Preview)

Upon release, the CLI will allow you to run a scan directly against your project directory. The AST engine analyzes your agent graph and MCP manifests.

```bash
# Run a standard scan in the current directory
orvyen scan .

# Run in CI mode (returns non-zero exit code on failures)
orvyen scan . --ci

# Generate an AIBOM compliance report in PDF format
orvyen scan . --format pdf --output aibom_report.pdf

```

## Output Formats

Orvyen Agentic will support multiple output formats depending on the deployment environment:

* Terminal output for local development (pass/fail, inline).


* JSON and HTML reports for CI/CD pipelines and dashboards.


* AIBOM PDF for compliance and audit handoff.
