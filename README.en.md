<h1 align="center">Hi, I'm Nicole de Carvalho 👋</h1>

<h3 align="center">💻 Full-Stack Developer &nbsp;·&nbsp; ☕ Java · 🐍 Python · 🟣 .NET &nbsp;·&nbsp; 🤖 Applied AI</h3>

<p align="center">🎓 <b>Software Engineering</b> (bachelor's) · expected graduation: second half of 2027 &nbsp;|&nbsp; 🇧🇷 <a href="https://github.com/nicole21carvalho"><b>Versão em português</b></a></p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3500&pause=800&color=BD93F9&center=true&vCenter=true&width=640&lines=AI+agents+with+LangGraph+and+MCP;Event-driven+microservices+with+Kafka;Event-sourced+banking+in+.NET;RAG+with+LangChain%2C+pgvector+and+Ollama;Docker%2C+Kubernetes+and+CI%2FCD" alt="AI agents, Kafka microservices, event sourcing in .NET, RAG and DevOps" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nicole-de-carvalho-7465b52a5" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:nicolerdcarvalho@gmail.com"><img src="https://img.shields.io/badge/E--mail-333333?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail"></a>
  <img src="https://img.shields.io/badge/Open%20to%20internships%20and%20jobs-2EA44F?style=for-the-badge" alt="Open to internships and jobs">
</p>

---

## 💡 About me

Full-stack developer focused on **back-end, distributed systems and applied AI**.

- 🤖 **AI with measured results**: an MCP agent evaluated with real models in CI (94% accuracy), RAG that cites the
  page each answer came from, and prompt-injection defenses
- 🏗️ **Systems that don't lose data**: sagas with Kafka, outbox, idempotency and event sourcing, with concurrency
  tested against a real PostgreSQL
- 🔐 **Security from the first commit**: OAuth 2.0 / OIDC with Keycloak, passkeys, token exchange (RFC 8693),
  non-root containers and CodeQL
- 🔭 **End-to-end observability**: OpenTelemetry traces across every service (one of them showed me a duplicate-order
  bug, which I fixed with idempotency)
- 🐧 **Linux every day**, with Docker, Kubernetes and GitHub Actions

> *Each project below has an English summary at the top of its README; the rest of the documentation is in
> Portuguese.*

---

## 🚀 Featured projects

<table>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/bazar-ai-agent-mcp#-in-english"><img src="https://raw.githubusercontent.com/nicole21carvalho/bazar-ai-agent-mcp/main/docs/img/chat-confirmacao.png" alt="The agent's chat in the Bazar store with the order confirmation card" width="100%"></a>
    </td>
    <td>
      <h3>🤖 <a href="https://github.com/nicole21carvalho/bazar-ai-agent-mcp#-in-english">Customer-service agent with MCP</a></h3>
      An AI agent that checks orders and places them <b>on behalf of the logged-in customer</b>, without ever passing their token along.
      <ul>
        <li>Custom MCP server + LangGraph agent, with <b>token exchange (RFC 8693)</b> at every hop</li>
        <li>Every purchase waits for <b>human confirmation</b> in the app</li>
        <li>Evaluated with real models in CI: <b>94% (15 of 16 scenarios)</b> on the default model</li>
        <li>An OpenTelemetry trace caught an order that could be created twice, fixed with an <code>Idempotency-Key</code></li>
      </ul>
      <code>Python</code> <code>LangGraph</code> <code>MCP</code> <code>FastAPI</code> <code>Ollama</code> <code>Keycloak</code> <code>OpenTelemetry</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/lastro-digital-bank-dotnet#-in-english"><img src="https://raw.githubusercontent.com/nicole21carvalho/lastro-digital-bank-dotnet/main/docs/img/aspire-trace-pix.png" alt="Trace of a Pix transfer in the .NET Aspire dashboard" width="100%"></a>
    </td>
    <td>
      <h3>🏦 <a href="https://github.com/nicole21carvalho/lastro-digital-bank-dotnet#-in-english">Lastro, a digital bank in .NET</a></h3>
      A bank where money never disappears or duplicates.
      <ul>
        <li><b>Double-entry ledger</b> with event sourcing: the sum of all balances is always zero</li>
        <li><b>Idempotent Pix</b> (Brazil's instant payments), the Central Bank's night-time limit and an outbox saga for other banks</li>
        <li>Concurrency proven on PostgreSQL: <b>400 crossed Pix and 250 parallel deposits</b>, with no deadlock</li>
        <li>Passkeys, anti-fraud and audit trail; <b>130 tests</b> and CodeQL in CI</li>
      </ul>
      <code>C#</code> <code>.NET 10</code> <code>Marten</code> <code>PostgreSQL</code> <code>Keycloak</code> <code>.NET Aspire</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/bazar-microservices-kafka#-in-english"><img src="https://raw.githubusercontent.com/nicole21carvalho/bazar-microservices-kafka/main/docs/img/painel.png" alt="The Bazar dashboard with an order going through the saga steps" width="100%"></a>
    </td>
    <td>
      <h3>🛍️ <a href="https://github.com/nicole21carvalho/bazar-microservices-kafka#-in-english">Bazar, an event-driven store</a></h3>
      A store that never loses an order, even when a service goes down mid-purchase.
      <ul>
        <li>5 Java services with <b>Kafka</b>: saga with compensation, <b>Transactional Outbox</b> and idempotent consumers</li>
        <li>Every order becomes a trace across all services (Jaeger + Grafana)</li>
        <li><b>Kubernetes, Terraform and GitOps (Flux)</b> for Oracle Cloud, tested on a local k3s</li>
        <li><b>42 integration tests</b> with real Postgres and Kafka, 25 front-end tests and 15 end-to-end checks</li>
      </ul>
      <code>Java 25</code> <code>Spring Boot</code> <code>Kafka</code> <code>React</code> <code>TypeScript</code> <code>Kubernetes</code> <code>Terraform</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/rag-pdf-chat-citations#-in-english"><img src="https://raw.githubusercontent.com/nicole21carvalho/rag-pdf-chat-citations/main/docs/img/conversa.png" alt="Oráculo answering a question about a PDF, with page citations" width="100%"></a>
    </td>
    <td>
      <h3>🔮 <a href="https://github.com/nicole21carvalho/rag-pdf-chat-citations#-in-english">Oráculo, ask your PDFs</a></h3>
      RAG that answers questions about your documents and <b>cites the page</b> each piece of information came from.
      <ul>
        <li>Vector search evaluated with known-answer questions: <b>right page ranked first in 11 of 12</b></li>
        <li>Streamed answers and AI running locally with Ollama</li>
        <li>Prompt-injection defenses, Argon2 and Kubernetes deployment</li>
      </ul>
      <code>Python</code> <code>FastAPI</code> <code>LangChain</code> <code>pgvector</code> <code>Next.js</code> <code>Kubernetes</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/ai-expense-tracker#-in-english"><img src="https://raw.githubusercontent.com/nicole21carvalho/ai-expense-tracker/main/docs/img/painel.png" alt="The Cofre dashboard with the month's balance and categorized statement" width="100%"></a>
    </td>
    <td>
      <h3>💰 <a href="https://github.com/nicole21carvalho/ai-expense-tracker#-in-english">Cofre, personal finance</a></h3>
      You log the expense, Cofre figures out the category.
      <ul>
        <li>Categorization by a <b>language model</b>, with a rule-based classifier when there is no API key</li>
        <li>The AI's answer is validated before saving, and a network failure means "no suggestion", not an error</li>
        <li>Spring Security, PostgreSQL and Docker</li>
      </ul>
      <code>Java 21</code> <code>Spring Boot</code> <code>Angular</code> <code>PostgreSQL</code> <code>Docker</code>
    </td>
  </tr>
</table>

<details>
  <summary><b>🌐 More projects: published websites and data analysis</b></summary>
  <br>

| Project | What it is | Links |
|---|---|---|
| 🌦️ **Weather and Highway Accidents** | How weather affects accidents on Brazilian federal highways (open data from the PRF), with an interactive dashboard | [Code](https://github.com/nicole21carvalho/projeto_efeito_clima) |
| 🏦 **Tech.In.Fin Bank** | Digital bank website with a customer area, Pix and forms with digital signature | [Site](https://nicole21carvalho.github.io/Site-de-banco/) · [Code](https://github.com/nicole21carvalho/Site-de-banco) |
| 🏥 **Flu Symptom Triage** | Form with CPF validation, input masks and a triage summary | [Site](https://nicole21carvalho.github.io/hospital-flu-screening-form/) · [Code](https://github.com/nicole21carvalho/hospital-flu-screening-form) |
| 🛒 **Sales Dashboard** | Sales dashboard with filters, indicators and charts | [Site](https://nicole21carvalho.github.io/Cadastro-de-Vendas/) · [Code](https://github.com/nicole21carvalho/Cadastro-de-Vendas) |
| 🧮 **Calculator** | Calculator without eval, with keyboard support and tests | [Site](https://nicole21carvalho.github.io/Calculadora/) · [Code](https://github.com/nicole21carvalho/Calculadora) |
| 🛗 **11-Stop Elevator** | Elevator simulation with a floor queue and animation | [Site](https://nicole21carvalho.github.io/Elevador-11-paradas/) · [Code](https://github.com/nicole21carvalho/Elevador-11-paradas) |
| 🛍️ **CCI Store** | Product catalog REST API, with tests and CI | [Code](https://github.com/nicole21carvalho/ecommerce-spring-boot-api) |

</details>

---

## 🛠️ Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,cs,dotnet,ts,react,angular,nextjs&perline=10" alt="Java, Spring, Python, FastAPI, C#, .NET, TypeScript, React, Angular and Next.js" />
  <br>
  <img src="https://skillicons.dev/icons?i=postgres,redis,kafka,docker,kubernetes,terraform,githubactions,grafana,linux,bash&perline=10" alt="PostgreSQL, Redis, Kafka, Docker, Kubernetes, Terraform, GitHub Actions, Grafana, Linux and Bash" />
</p>

<p align="center">
  <b>🤖 AI</b><br>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white" alt="MCP (Model Context Protocol)" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama" />
  <img src="https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector" />
  <img src="https://img.shields.io/badge/RAG-8E44AD?style=for-the-badge" alt="RAG" />
  <img src="https://img.shields.io/badge/OpenTelemetry%20GenAI-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white" alt="OpenTelemetry GenAI" />
</p>

<div align="center">

| Area | Technologies |
|:--|:--|
| 💻 **Languages** | Java · Python · C# · TypeScript · JavaScript · SQL · C · HTML · CSS |
| ⚙️ **Back-end** | Spring Boot · FastAPI · ASP.NET Core · Node.js · Kafka · Keycloak (OAuth 2.0 / OIDC) |
| 🎨 **Front-end** | React · Angular · Next.js · Tailwind CSS |
| 🤖 **AI** | LangGraph · LangChain · MCP · RAG · embeddings · pgvector · Ollama · LLM evaluation |
| 🗄️ **Data** | PostgreSQL · Redis · MySQL · event sourcing (Marten) · Pandas · Streamlit |
| 🚀 **DevOps** | Docker · Kubernetes · Terraform · GitHub Actions · OpenTelemetry · Prometheus · Grafana |
| 🐧 **Linux & Networking** | Linux · Bash · computer networks · Wireshark |

</div>

## 📚 Currently learning

- **Already using in projects:** tool-using agents (MCP), RAG, embeddings and vector search, model evaluation,
  AI tracing with OpenTelemetry
- **Going deeper:** reranking, fine-tuning, Spring AI and Hugging Face

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=nicole21carvalho&layout=compact&langs_count=8&theme=dracula&locale=en&hide_border=true" height="150" alt="Most used languages in my repositories" />
</p>
