<div align="center">

<img src="assets/banner.svg" alt="Joel Oyewole. I build AI agents and backends that connect to the tools a business already uses." width="100%">

<br>

<img src="assets/stack.svg" alt="Stack: Python, FastAPI, PostgreSQL, LLM APIs (OpenAI-compatible), RAG, MCP, Docker" width="86%">

<br><br>

<a href="https://x.com/joel_depin"><b>Follow on X</b></a> &nbsp;·&nbsp; <a href="#what-i-build-for-clients"><b>For clients</b></a> &nbsp;·&nbsp; <a href="#engineering-projects"><b>Engineering</b></a> &nbsp;·&nbsp; <a href="#building"><b>Building</b></a>

<img src="assets/divider.svg" alt="" width="100%">

</div>

## What I build for clients

Working tools for real business problems. Each one comes with source code, a README with a quickstart and a test suite, and I can adapt it to your data.

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/catalog-chat-assistant"><img src="assets/catalog-chat-assistant.png" alt="catalog-chat-assistant: two shops, each with its own chat grounded in its catalog" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/catalog-chat-assistant">catalog-chat-assistant</a></h3>
A shopping assistant that answers only from a shop's own product catalog: recommendations, comparisons and "which items are vegan under $5?". Says so when something isn't in the catalog, and each shop's data stays separate.
<br><sub><b>Chatbot · tool calling · ChromaDB · multi-tenant</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/docs-rag-chatbot"><img src="assets/docs-rag-chatbot.png" alt="docs-rag-chatbot: a chat answering a question with a clickable page citation" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/docs-rag-chatbot">docs-rag-chatbot</a></h3>
Answers questions over company documents, with citations to the source page. Click a citation and the PDF opens at that page. A question the documents don't cover gets an honest "I couldn't find that".
<br><sub><b>RAG · ChromaDB · FastAPI · Groq</b></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/invoice-extractor"><img src="assets/invoice-extractor.png" alt="invoice-extractor: an invoice flagged for review because the total does not add up" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/invoice-extractor">invoice-extractor</a></h3>
Turns messy PDF invoices into validated structured JSON. Confidence on every field, and arithmetic errors are flagged for review, never silently fixed.
<br><sub><b>FastAPI · Pydantic · LLM extraction · validation</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/product-data-extractor"><img src="assets/product-data-extractor.png" alt="product-data-extractor: six product pages extracted with per-field sources" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/product-data-extractor">product-data-extractor</a></h3>
Paste a product page URL and get clean structured data, optionally filled into a Google Sheets row. Standard page data first, an LLM only for gaps, and every field shows its source.
<br><sub><b>Web extraction · schema.org · Google Sheets</b></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/web-flow-bot"><img src="assets/web-flow-bot.png" alt="web-flow-bot: a real run where two 503 errors were retried and the confirmation verified" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/web-flow-bot">web-flow-bot</a></h3>
Playwright bot that logs in, fills a form, submits it and verifies the confirmation number. Retries with backoff, a screenshot of every attempt and a JSON run log.
<br><sub><b>Playwright · retries · Docker · pytest</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/llm-cost-router"><img src="assets/llm-cost-router.png" alt="llm-cost-router: benchmark report from a real run" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/llm-cost-router">llm-cost-router</a></h3>
Sends each prompt to the cheapest model that passes a quality check, escalates only on failure and caches repeats. Prices come from config, and the benchmark reports only what a real run measured.
<br><sub><b>OpenAI-compatible APIs · routing · caching</b></sub>
</td>
</tr>
</table>

<div align="center"><img src="assets/divider.svg" alt="" width="100%"></div>

## Engineering projects

How I build the foundations: auth and billing, safety for AI agents, protocols and tool use. These show how I work rather than a product to buy.

<table>
<tr>
<td width="33%" valign="top">
<a href="https://github.com/joel819/fastapi-saas-backend"><img src="assets/fastapi-saas-backend.png" alt="fastapi-saas-backend: a playground showing the premium gate, checkout and webhook replay" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/fastapi-saas-backend">fastapi-saas-backend</a></h3>
JWT auth with rotating refresh tokens, subscriptions, verified and idempotent Stripe webhooks, rate limiting and a full test suite.
<br><sub><b>FastAPI · JWT · Stripe · SQLAlchemy</b></sub>
</td>
<td width="33%" valign="top">
<a href="https://github.com/joel819/agent-spend-guard"><img src="assets/agent-spend-guard.png" alt="agent-spend-guard: a dashboard with a daily cap meter and an approval queue" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/agent-spend-guard">agent-spend-guard</a></h3>
Spend limits and human approval for AI agents that handle funds, with a tamper-evident audit log.
<br><sub><b>FastAPI · policy as config · audit log</b></sub>
</td>
<td width="33%" valign="top">
<a href="https://github.com/joel819/mcp-server-template"><img src="assets/mcp-server-template.png" alt="mcp-server-template: an MCP explorer page" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/mcp-server-template">mcp-server-template</a></h3>
An MCP server exposing a real API as a tool for any agent. Streamable HTTP and stdio from one definition.
<br><sub><b>MCP · GitHub API · stdio</b></sub>
</td>
</tr>
<tr>
<td width="33%" valign="top">
<a href="https://github.com/joel819/support-agent"><img src="assets/support-agent.png" alt="support-agent: answers tagged with the route taken" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/support-agent">support-agent</a></h3>
Support agent combining document search with live order lookups via tool calling. Every answer shows its route and tool calls.
<br><sub><b>Tool calling · RAG · routing log</b></sub>
</td>
<td width="33%" valign="top">
<a href="https://github.com/joel819/sandboxed-agent"><img src="assets/sandboxed-agent.png" alt="sandboxed-agent: the policy drawn as a fence around the agent" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/sandboxed-agent">sandboxed-agent</a></h3>
Runs support-agent inside an NVIDIA OpenShell sandbox with an allow-list policy for files and network.
<br><sub><b>OpenShell · policy as code · Docker</b></sub>
</td>
<td></td>
</tr>
</table>

<div align="center"><img src="assets/divider.svg" alt="" width="100%"></div>

## How I build

<table>
<tr>
<td width="33%" valign="top">
<b>Easy to run</b><br>
Each README has a short quickstart, and the AI projects have a demo mode or a free-tier setup, so you can see them working in minutes.
</td>
<td width="33%" valign="top">
<b>Tested offline</b><br>
Test suites that need no keys, no model download and no network, so they run anywhere.
</td>
<td width="33%" valign="top">
<b>Honest about failure</b><br>
Low-confidence flags instead of silent fixes, hard rejects with the numbers, "I couldn't find that" instead of a guess.
</td>
</tr>
</table>

<div align="center"><img src="assets/divider.svg" alt="" width="100%"></div>

## Building

**SoverGrid**: a routing layer for decentralized compute.

## Contact

[X (@joel_depin)](https://x.com/joel_depin)
