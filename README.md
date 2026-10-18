<h1 align="center">Olá, eu sou a Nicole de Carvalho 👋</h1>

<h3 align="center">💻 Desenvolvedora Full Stack &nbsp;·&nbsp; ☕ Java · 🐍 Python · 🟣 .NET &nbsp;·&nbsp; 🤖 IA aplicada</h3>

<p align="center">🎓 <b>Engenharia de Software</b> · formatura prevista em 2027.2 &nbsp;|&nbsp; 🌎 <a href="https://github.com/nicole21carvalho/nicole21carvalho/blob/main/README.en.md"><b>Read in English</b></a></p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3500&pause=800&color=BD93F9&center=true&vCenter=true&width=640&lines=Agentes+de+IA+com+LangGraph+e+MCP;Microsservi%C3%A7os+com+Kafka+e+sagas;Banco+digital+com+event+sourcing+em+.NET;RAG+com+LangChain%2C+pgvector+e+Ollama;Docker%2C+Kubernetes+e+CI%2FCD" alt="Agentes de IA, microsserviços com Kafka, event sourcing em .NET, RAG e DevOps" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nicole-de-carvalho-7465b52a5" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:nicolerdcarvalho@gmail.com"><img src="https://img.shields.io/badge/E--mail-333333?style=for-the-badge&logo=gmail&logoColor=white" alt="E-mail"></a>
  <img src="https://img.shields.io/badge/Aberta%20a%20est%C3%A1gios%20e%20vagas-2EA44F?style=for-the-badge" alt="Aberta a estágios e vagas">
</p>

---

## 💡 Sobre mim

Desenvolvedora full stack com foco em **back-end, sistemas distribuídos e IA aplicada**.

- 🤖 **IA com resultado medido**: agente com MCP avaliado com modelos reais no CI (94% de acerto), RAG que cita a
  página de onde veio cada resposta e defesa contra *prompt injection*
- 🏗️ **Sistemas que não perdem dados**: sagas com Kafka, outbox, idempotência e event sourcing, com concorrência
  testada no PostgreSQL de verdade
- 🔐 **Segurança desde o primeiro commit**: OAuth 2.0 / OIDC com Keycloak, passkeys, troca de token (RFC 8693),
  containers sem root e CodeQL
- 🔭 **Observabilidade de ponta a ponta**: *traces* do OpenTelemetry que atravessam todos os serviços (foi um deles
  que me mostrou um bug de pedido em dobro, que corrigi com idempotência)
- 🐧 **Linux no dia a dia**, com Docker, Kubernetes e GitHub Actions

> 🌎 *Full-stack developer (Java · Python · .NET · AI), open to internships and job opportunities.
> [Full profile in English](https://github.com/nicole21carvalho/nicole21carvalho/blob/main/README.en.md); every
> project below has an English summary at the top.*

---

## 🚀 Projetos em destaque

<table>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/bazar-ai-agent-mcp"><img src="https://raw.githubusercontent.com/nicole21carvalho/bazar-ai-agent-mcp/main/docs/img/chat-confirmacao.png" alt="Chat do agente no painel do Bazar com o cartão de confirmação do pedido" width="100%"></a>
    </td>
    <td>
      <h3>🤖 <a href="https://github.com/nicole21carvalho/bazar-ai-agent-mcp">Agente de atendimento com MCP</a></h3>
      Agente de IA que consulta pedidos e faz compras <b>em nome do cliente logado</b>, sem nunca repassar o token dele.
      <ul>
        <li>Servidor MCP próprio + agente LangGraph, com <b>troca de token (RFC 8693)</b> a cada salto</li>
        <li>Toda compra espera a <b>confirmação humana</b> no app</li>
        <li>Avaliado com modelos reais no CI: <b>94% (15 de 16 cenários)</b> no modelo padrão</li>
        <li>O <i>trace</i> do OpenTelemetry achou um pedido que podia sair em dobro, corrigido com <code>Idempotency-Key</code></li>
      </ul>
      <code>Python</code> <code>LangGraph</code> <code>MCP</code> <code>FastAPI</code> <code>Ollama</code> <code>Keycloak</code> <code>OpenTelemetry</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/lastro-digital-bank-dotnet"><img src="https://raw.githubusercontent.com/nicole21carvalho/lastro-digital-bank-dotnet/main/docs/img/aspire-trace-pix.png" alt="Trace de um Pix no painel do .NET Aspire" width="100%"></a>
    </td>
    <td>
      <h3>🏦 <a href="https://github.com/nicole21carvalho/lastro-digital-bank-dotnet">Lastro, banco digital em .NET</a></h3>
      Banco em que o dinheiro nunca some nem duplica.
      <ul>
        <li><b>Livro-razão com partidas dobradas</b> e event sourcing: a soma de todos os saldos é sempre zero</li>
        <li><b>Pix idempotente</b>, limite noturno do Banco Central e saga com outbox para outros bancos</li>
        <li>Concorrência provada no PostgreSQL: <b>400 Pix cruzados e 250 depósitos em paralelo</b>, sem travar</li>
        <li>Passkeys, antifraude e auditoria; <b>130 testes</b> e CodeQL no CI</li>
      </ul>
      <code>C#</code> <code>.NET 10</code> <code>Marten</code> <code>PostgreSQL</code> <code>Keycloak</code> <code>.NET Aspire</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/bazar-microservices-kafka"><img src="https://raw.githubusercontent.com/nicole21carvalho/bazar-microservices-kafka/main/docs/img/painel.png" alt="Painel do Bazar com um pedido passando pelas etapas da saga" width="100%"></a>
    </td>
    <td>
      <h3>🛍️ <a href="https://github.com/nicole21carvalho/bazar-microservices-kafka">Bazar, loja em microsserviços</a></h3>
      Loja que nunca perde um pedido, mesmo com serviço caindo no meio da compra.
      <ul>
        <li>5 serviços Java com <b>Kafka</b>: saga com compensação, <b>Transactional Outbox</b> e consumo idempotente</li>
        <li>Cada pedido vira um <i>trace</i> que atravessa todos os serviços (Jaeger + Grafana)</li>
        <li><b>Kubernetes, Terraform e GitOps (Flux)</b> para a Oracle Cloud, testados num k3s local</li>
        <li><b>42 testes de integração</b> com Postgres e Kafka de verdade, 25 no front-end e 15 de ponta a ponta</li>
      </ul>
      <code>Java 25</code> <code>Spring Boot</code> <code>Kafka</code> <code>React</code> <code>TypeScript</code> <code>Kubernetes</code> <code>Terraform</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/rag-pdf-chat-citations"><img src="https://raw.githubusercontent.com/nicole21carvalho/rag-pdf-chat-citations/main/docs/img/conversa.png" alt="Oráculo respondendo uma pergunta sobre um PDF, com citações das páginas" width="100%"></a>
    </td>
    <td>
      <h3>🔮 <a href="https://github.com/nicole21carvalho/rag-pdf-chat-citations">Oráculo, perguntas sobre PDFs</a></h3>
      RAG que responde sobre os seus documentos e <b>cita a página</b> de onde tirou cada informação.
      <ul>
        <li>Busca vetorial avaliada com perguntas de resposta conhecida: <b>página certa em 1º lugar em 11 de 12</b></li>
        <li>Resposta em tempo real (streaming) e IA rodando localmente com Ollama</li>
        <li>Defesa contra <i>prompt injection</i>, Argon2 e deploy em Kubernetes</li>
      </ul>
      <code>Python</code> <code>FastAPI</code> <code>LangChain</code> <code>pgvector</code> <code>Next.js</code> <code>Kubernetes</code>
    </td>
  </tr>
  <tr>
    <td width="42%">
      <a href="https://github.com/nicole21carvalho/ai-expense-tracker"><img src="https://raw.githubusercontent.com/nicole21carvalho/ai-expense-tracker/main/docs/img/painel.png" alt="Painel do Cofre com saldo do mês e extrato categorizado" width="100%"></a>
    </td>
    <td>
      <h3>💰 <a href="https://github.com/nicole21carvalho/ai-expense-tracker">Cofre, controle financeiro</a></h3>
      Você lança o gasto, o Cofre descobre a categoria.
      <ul>
        <li>Categorização por <b>modelo de linguagem</b>, com classificador por regras quando não há chave de API</li>
        <li>A resposta da IA é validada antes de gravar, e falha de rede vira "sem sugestão", não erro</li>
        <li>Spring Security, PostgreSQL e Docker</li>
      </ul>
      <code>Java 21</code> <code>Spring Boot</code> <code>Angular</code> <code>PostgreSQL</code> <code>Docker</code>
    </td>
  </tr>
</table>

<details>
  <summary><b>🌐 Mais projetos: sites publicados e análise de dados</b></summary>
  <br>

| Projeto | O que é | Links |
|---|---|---|
| 🌦️ **Efeito do Clima nas Rodovias** | Análise do impacto do clima nos acidentes em rodovias federais (dados abertos da PRF), com painel interativo | [Código](https://github.com/nicole21carvalho/projeto_efeito_clima) |
| 🏦 **Banco Tech.In.Fin** | Banco digital com área do cliente, Pix e formulários com assinatura digital | [Site](https://nicole21carvalho.github.io/Site-de-banco/) · [Código](https://github.com/nicole21carvalho/Site-de-banco) |
| 🏥 **Triagem de Sintomas Gripais** | Formulário com validação de CPF, máscaras e resumo da triagem | [Site](https://nicole21carvalho.github.io/hospital-flu-screening-form/) · [Código](https://github.com/nicole21carvalho/hospital-flu-screening-form) |
| 🛒 **Cadastro de Vendas** | Dashboard de vendas com filtros, indicadores e gráficos | [Site](https://nicole21carvalho.github.io/Cadastro-de-Vendas/) · [Código](https://github.com/nicole21carvalho/Cadastro-de-Vendas) |
| 🧮 **Calculadora** | Calculadora sem eval, com suporte ao teclado e testes | [Site](https://nicole21carvalho.github.io/Calculadora/) · [Código](https://github.com/nicole21carvalho/Calculadora) |
| 🛗 **Elevador de 11 paradas** | Simulação de elevador com fila de andares e animação | [Site](https://nicole21carvalho.github.io/Elevador-11-paradas/) · [Código](https://github.com/nicole21carvalho/Elevador-11-paradas) |
| 🛍️ **Loja CCI** | API REST de catálogo de produtos, com testes e CI | [Código](https://github.com/nicole21carvalho/ecommerce-spring-boot-api) |

</details>

---

## 🛠️ Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,cs,dotnet,ts,react,angular,nextjs&perline=10" alt="Java, Spring, Python, FastAPI, C#, .NET, TypeScript, React, Angular e Next.js" />
  <br>
  <img src="https://skillicons.dev/icons?i=postgres,redis,kafka,docker,kubernetes,terraform,githubactions,grafana,linux,bash&perline=10" alt="PostgreSQL, Redis, Kafka, Docker, Kubernetes, Terraform, GitHub Actions, Grafana, Linux e Bash" />
</p>

<p align="center">
  <b>🤖 IA</b><br>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge&logo=modelcontextprotocol&logoColor=white" alt="MCP (Model Context Protocol)" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama" />
  <img src="https://img.shields.io/badge/pgvector-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector" />
  <img src="https://img.shields.io/badge/RAG-8E44AD?style=for-the-badge" alt="RAG" />
  <img src="https://img.shields.io/badge/OpenTelemetry%20GenAI-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white" alt="OpenTelemetry GenAI" />
</p>

<div align="center">

| Área | Tecnologias |
|:--|:--|
| 💻 **Linguagens** | Java · Python · C# · TypeScript · JavaScript · SQL · C · HTML · CSS |
| ⚙️ **Back-end** | Spring Boot · FastAPI · ASP.NET Core · Node.js · Kafka · Keycloak (OAuth 2.0 / OIDC) |
| 🎨 **Front-end** | React · Angular · Next.js · Tailwind CSS |
| 🤖 **IA** | LangGraph · LangChain · MCP · RAG · embeddings · pgvector · Ollama · avaliação de LLMs |
| 🗄️ **Dados** | PostgreSQL · Redis · MySQL · event sourcing (Marten) · Pandas · Streamlit |
| 🚀 **DevOps** | Docker · Kubernetes · Terraform · GitHub Actions · OpenTelemetry · Prometheus · Grafana |
| 🐧 **Linux & Redes** | Linux · Bash · redes de computadores · Wireshark |

</div>

## 📚 Estudando agora

- **Já uso em projeto:** agentes com ferramentas (MCP), RAG, embeddings e busca vetorial, avaliação de modelos,
  rastreamento de IA com OpenTelemetry
- **Aprofundando:** reranking, fine-tuning, Spring AI e Hugging Face

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=nicole21carvalho&layout=compact&langs_count=8&theme=dracula&locale=pt-br&hide_border=true" height="150" alt="Linguagens mais usadas nos meus repositórios" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/nicole21carvalho/nicole21carvalho/output/snake.svg" alt="Animação da cobrinha comendo o gráfico de contribuições" />
</p>
