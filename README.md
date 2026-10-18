<p align="center">
  <img src="assets/shini-banner-v1.png" width="100%" alt="Shini — AI Engineer. White-haired anime character holding a shark plush, in ice-blue tones.">
</p>

<p align="center">
  <samp>RETRIEVAL · AGENTS · LLM SYSTEMS · AI SECURITY</samp><br>
  <sub>Доверяй, но проверяй.</sub>
</p>

<p align="center">
  <a href="#engineering">Engineering</a> &nbsp; / &nbsp;
  <a href="#toolbox">Toolbox</a> &nbsp; / &nbsp;
  <a href="#selected-work">Selected work</a> &nbsp; / &nbsp;
  <a href="#off-duty">Вне смены</a>
</p>

<table width="100%">
<tr>
<td width="76%" valign="middle">
<h3>Shini / AI Engineer &amp; Tech Lead</h3>
<p>I work on agents, retrieval and the platform around them. C/Assembly, embedded systems and automation were my starting point. My work now spans model integration, shared backend services and hybrid Azure/GCP environments.</p>
<p><strong>I put LLMs in production.<br>I still don't trust them.</strong></p>
</td>
<td width="24%" align="center" valign="middle">
<a href="https://giphy.com/gifs/sad-gawr-gura-absurdexcrod-FN6731cXHeb7VJCkly"><img src="assets/gura-pain.gif" width="144" alt="Gura looking unimpressed, with the caption PAIN."></a>
<br><sub>Всё под контролем.<br>Probably.</sub>
</td>
</tr>
</table>

## Engineering

<sub>01 / TECHNICAL FOCUS — WHAT I PAY ATTENTION TO</sub>

<table width="100%">
<tr>
<td width="50%" valign="top">
<sub>01.1 / RETRIEVAL</sub>
<h3>Advanced RAG</h3>
<p>Hybrid search, reranking, evidence selection and semantic caching. Document structure and provenance before index tuning.</p>
<p><code>Recall@k</code> · <code>MRR</code> · <code>grounding</code> · <code>abstention</code></p>
</td>
<td width="50%" valign="top">
<sub>01.2 / ORCHESTRATION</sub>
<h3>Agentic systems</h3>
<p>Explicit graph state, typed tools and bounded planning loops. Checkpoints, idempotent actions and a stopping condition.</p>
<p><code>state</code> · <code>tool contracts</code> · <code>permissions</code></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<sub>01.3 / MODEL SYSTEMS</sub>
<h3>LLM engineering</h3>
<p>Validated outputs, prompt and model versioning, regression datasets and provider fallbacks. Quality, latency and cost in the same release decision.</p>
<p><code>evals</code> · <code>tracing</code> · <code>fallbacks</code></p>
</td>
<td width="50%" valign="top">
<sub>01.4 / TRUST BOUNDARIES</sub>
<h3>AI security engineering</h3>
<p>Prompt injection, retrieval-based exfiltration, tool abuse and cross-tenant access. Scoped credentials and repeatable adversarial tests.</p>
<p><code>authorization</code> · <code>isolation</code> · <code>red teaming</code></p>
</td>
</tr>
</table>

<details>
<summary><strong>Open the design notes</strong> — retrieval, execution and security</summary>

### Retrieval & evidence

Parsing, chunking and provenance are separate stages. Evaluate retrieval and generation independently; inspect evidence and citation grounding, including queries that should produce an abstention.

### Agent execution

Tool contracts define what an agent can do. State, checkpoints, idempotency and approval boundaries define what happens when execution fails or crosses into an external system.

### LLM releases

Version prompts, models and evaluation datasets together. Compare quality, latency and inference cost before promotion; keep a fallback and a rollback path.

### Security boundaries

Apply authorization at retrieval and tool boundaries. Treat retrieved content and tool output as untrusted input. Handle sensitive data in traces deliberately and turn abuse cases into repeatable tests.

</details>

## Toolbox

<sub>02 / APPLICATIONS → PLATFORM → OPERATIONS</sub>

| Layer | Stack |
| :--- | :--- |
| **Application & systems** | Python · FastAPI · TypeScript · C/Assembly |
| **AI & retrieval** | LangChain / LangGraph · PyTorch · Vertex AI · PostgreSQL / pgvector · BM25 · reranking |
| **Cloud & platform** | GCP · GKE / Kubernetes · Azure · Docker · Secret Manager |
| **Data & messaging** | PostgreSQL · Kafka |
| **Evaluation & delivery** | OpenTelemetry · regression evaluations · shadow mode · Azure DevOps |

<sub>Digging deeper: C++ · inference serving · durable agent execution.</sub>

## Selected work

<sub>03 / READ THE CODE, CHECK THE TRADE-OFFS</sub>

<table width="100%">
<tr>
<td width="50%" valign="top">
<sub>AGENTIC RETRIEVAL</sub>
<h3><a href="https://github.com/CallmeShini/nextjs-docs-rag">nextjs-docs-rag ↗</a></h3>
<p>Agentic retrieval over Next.js documentation: hybrid search, local reranking, evidence memory and semantic caching.</p>
<p><strong>Inspect:</strong> explicit orchestration and reproducible cold/warm benchmarks.</p>
</td>
<td width="50%" valign="top">
<sub>GROUNDED DOCUMENTATION QA</sub>
<h3><a href="https://github.com/CallmeShini/docsrag-observatory">docsrag-observatory ↗</a></h3>
<p>Documentation QA with a deterministic data pipeline, explicit abstention and separate evaluation of retrieval and generation.</p>
<p><strong>Inspect:</strong> provenance, answer gating and evaluation-driven iteration.</p>
</td>
</tr>
</table>

## Off duty

<details>
<summary><strong>За кулисами</strong> / behind the scenes</summary>

Меньше суеты. Больше работающего кода.<br>
Акула отвечает за моральную поддержку. За код отвечаю я.

</details>

<p align="center">
  <sub>На связи. / The shark is emotional support. I review the code.</sub><br>
  <sub>GIF: <a href="https://giphy.com/gifs/sad-gawr-gura-absurdexcrod-FN6731cXHeb7VJCkly">Nosenzei via GIPHY</a></sub>
</p>
