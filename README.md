<div align="center">

<img src="assets/banner.svg" alt="Joel Oyewole. I build AI agents and backends that connect to the tools a business already uses." width="100%">

<br>

<img src="assets/stack.svg" alt="Stack: Python, FastAPI, PostgreSQL, LLM APIs (OpenAI-compatible), RAG, MCP, Docker" width="86%">

<br><br>

<a href="https://x.com/joel_depin"><b>Follow on X</b></a> &nbsp;·&nbsp; <a href="#selected-work"><b>Selected work</b></a> &nbsp;·&nbsp; <a href="#building"><b>Building</b></a>

<img src="assets/divider.svg" alt="" width="100%">

</div>

## Selected work

Every project below runs locally for free, with a demo mode that needs no API keys, and has an offline test suite.

<table>
<tr>
<td colspan="2" align="center">
<a href="https://github.com/joel819/docs-rag-chatbot"><img src="assets/docs-rag-chatbot.png" alt="docs-rag-chatbot: a chat answering a question with a clickable page citation" width="100%"></a>
<br><br>
<h3><a href="https://github.com/joel819/docs-rag-chatbot">docs-rag-chatbot</a></h3>
Answers questions over company documents, with citations to the source page. Click a citation and the PDF opens at that page. A question the documents don't cover gets an honest "I couldn't find that" instead of a guess.
<br><sub><b>FastAPI · ChromaDB · RAG · sentence-transformers · Groq</b></sub>
<br><br>
</td>
</tr>
<tr>
<td colspan="2" align="center">
<a href="https://github.com/joel819/product-data-extractor"><img src="assets/product-data-extractor.png" alt="product-data-extractor: the output of its demo, six product pages extracted with per-field sources, and one page filled in by the LLM fallback" width="100%"></a>
<br><br>
<h3><a href="https://github.com/joel819/product-data-extractor">product-data-extractor</a></h3>
Paste a product page URL, get clean structured product data back, and optionally auto-fill a Google Sheets row. It reads the standard markup shops already publish (JSON-LD, Open Graph, microdata) and only asks an LLM for what is still missing, keeping only values that appear in the page text. Anything not found stays empty, and every field says where it came from and how much to trust it.
<br><sub><b>FastAPI · schema.org · SSRF-safe fetching · LLM fallback · Google Sheets (Apps Script)</b></sub>
<br><br>
</td>
</tr>
<tr>
<td colspan="2" align="center">
<a href="https://github.com/joel819/catalog-chat-assistant"><img src="assets/catalog-chat-assistant.png" alt="catalog-chat-assistant: two shops, a café and a bookshop, each with its own catalog-grounded chat, showing product cards and the tool calls behind each answer" width="100%"></a>
<br><br>
<h3><a href="https://github.com/joel819/catalog-chat-assistant">catalog-chat-assistant</a></h3>
A multi-tenant chat assistant that answers only from a business's own product catalog: recommendations, comparisons and "which items are vegan under $5?" lookups. The model works through search, filter and lookup tools instead of being handed the catalog, a question the catalog can't answer gets an honest "not in our catalog", and one shop can never see another's products.
<br><sub><b>FastAPI · tool calling · ChromaDB · sentence-transformers · multi-tenant · Groq</b></sub>
<br><br>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/web-flow-bot"><img src="assets/web-flow-bot.png" alt="web-flow-bot: screenshots from a real run in which the bot hit two 503 errors, retried with backoff and still verified the confirmation number" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/web-flow-bot">web-flow-bot</a></h3>
Playwright bot that logs in, fills a multi-field form, submits it and verifies the confirmation reference number. Per-step retries with backoff, a screenshot of every attempt and a JSON run log. Runs against a local demo site that can fail on purpose.
<br><sub><b>Playwright · FastAPI · retries · Docker · pytest</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/llm-cost-router"><img src="assets/llm-cost-router.png" alt="llm-cost-router: benchmark report from a real run, 50 prompts, always-strongest versus routed" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/llm-cost-router">llm-cost-router</a></h3>
Sends each prompt to the cheapest model that passes a quality check, escalates only on failure, caches repeats and logs cost per request. Prices come from config, never guesses, and the benchmark reports only what a real run measured.
<br><sub><b>OpenAI-compatible APIs · Groq · routing · caching · benchmark</b></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/support-agent"><img src="assets/support-agent.png" alt="support-agent: answers tagged with the route taken, with expandable tool calls" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/support-agent">support-agent</a></h3>
Support agent that combines document search with live order lookups via tool calling. Every answer shows the route it took and the exact tool calls behind it.
<br><sub><b>FastAPI · tool calling · RAG · routing log</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/invoice-extractor"><img src="assets/invoice-extractor.png" alt="invoice-extractor: an invoice flagged for review because the total does not add up" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/invoice-extractor">invoice-extractor</a></h3>
Turns messy PDF invoices into validated structured JSON through a FastAPI endpoint. Confidence on every field, and arithmetic errors are flagged for review, never silently fixed.
<br><sub><b>FastAPI · Pydantic · LLM extraction · validation</b></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/fastapi-saas-backend"><img src="assets/fastapi-saas-backend.png" alt="fastapi-saas-backend: a playground showing the premium gate, checkout and webhook replay" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/fastapi-saas-backend">fastapi-saas-backend</a></h3>
Production-style backend: JWT auth with rotating refresh tokens, subscriptions, verified and idempotent Stripe webhooks, rate limiting and a full test suite.
<br><sub><b>FastAPI · JWT · Stripe webhooks · SQLAlchemy</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/mcp-server-template"><img src="assets/mcp-server-template.png" alt="mcp-server-template: an MCP explorer page listing a repository's files" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/mcp-server-template">mcp-server-template</a></h3>
MCP server exposing a real API so any agent can use it as a tool. Streamable HTTP and stdio from one definition, with a built-in explorer page.
<br><sub><b>MCP · GitHub API · streamable HTTP · stdio</b></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/joel819/agent-spend-guard"><img src="assets/agent-spend-guard.png" alt="agent-spend-guard: a dashboard with a daily cap meter, a payment waiting for a human and a rejected payment" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/agent-spend-guard">agent-spend-guard</a></h3>
Spend limits and human approval for AI agents that handle funds. Auto-approve under a cap, a human decides above it, a hard reject at the daily limit, all in a tamper-evident audit log.
<br><sub><b>FastAPI · SQLite · policy as config · audit log</b></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/joel819/sandboxed-agent"><img src="assets/sandboxed-agent.png" alt="sandboxed-agent: the policy drawn as a fence around the agent" width="100%"></a>
<br>
<h3><a href="https://github.com/joel819/sandboxed-agent">sandboxed-agent</a></h3>
Runs support-agent inside an NVIDIA OpenShell sandbox: policy-restricted file and network access, with everything outside the allow-list blocked and logged.
<br><sub><b>NVIDIA OpenShell · policy as code · Docker</b></sub>
</td>
</tr>
</table>

<div align="center"><img src="assets/divider.svg" alt="" width="100%"></div>

## How I build

<table>
<tr>
<td width="33%" valign="top">
<b>Free to run</b><br>
Each project has a demo mode that works with no API keys, so anyone can clone it and see it working in a minute.
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
