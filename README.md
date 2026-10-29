<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg">
  <img src="./assets/header-dark.svg" alt="Leonardo Macedo — Desenvolvedor Full Stack" width="100%">
</picture>

<br/>

<a href="https://github.com/DevMacedojr">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=6C63FF&center=true&vCenter=true&width=640&lines=%3E+APIs+REST+e+integra%C3%A7%C3%B5es+entre+plataformas;%3E+Modelagem+e+otimiza%C3%A7%C3%A3o+SQL;%3E+Sistemas+legados+%E2%86%92+arquitetura+moderna;%3E+Linux+%C2%B7+Docker+%C2%B7+Nginx+%C2%B7+AWS;%3E+RAG+%C2%B7+LangChain+%C2%B7+Agentes+de+IA;%3E+Fluxos+de+conhecimento+especialista" alt="Typing SVG" />
</a>

<br/>

<img src="https://img.shields.io/badge/status-online-22C55E?style=flat-square&labelColor=0B0E14" alt="status" />
<img src="https://img.shields.io/badge/foco-sistemas_em_produção-6C63FF?style=flat-square&labelColor=0B0E14" alt="foco" />
<img src="https://img.shields.io/badge/local-Paraná,_BR-22D3EE?style=flat-square&labelColor=0B0E14" alt="local" />
<img src="https://komarev.com/ghpvc/?username=DevMacedojr&label=views&color=6C63FF&style=flat-square&labelColor=0B0E14" alt="views" />

<br/><br/>

<code><a href="#-sobre">./sobre</a></code> &nbsp;
<code><a href="#-competências">./competências</a></code> &nbsp;
<code><a href="#-stack">./stack</a></code> &nbsp;
<code><a href="#-ia-aplicada">./ia</a></code> &nbsp;
<code><a href="#-contato">./contato</a></code>

</div>

<br/>

## `$` sobre

```ts
const leonardo = {
  role:      "Desenvolvedor Full Stack",
  education: "Engenharia de Software (em andamento)",
  focus:     ["sistemas empresariais em produção", "APIs REST", "integrações", "legados"],
  infra:     ["Linux", "Docker", "Nginx", "AWS"],
  ai:        ["RAG", "LangChain", "agentes", "expert knowledge", "automação com LLMs"],
  mindset:   "entender a operação → localizar o gargalo → entregar algo que aguenta carga real",
};
```

> O que me interessa não é a stack, é o problema por trás dela.

<br/>

## `$` competências

<table>
<tr>
<td width="33%" valign="top">

**`01` · Aplicação**

```diff
+ Desenvolvimento Full Stack
+ APIs REST e integrações
+ Dashboards e painéis
+ Autenticação, JWT e permissões
```

</td>
<td width="33%" valign="top">

**`02` · Dados & infra**

```diff
+ Modelagem e otimização SQL
+ Servidores Linux e Nginx
+ Deploy, AWS e monitoramento
+ Containers com Docker
```

</td>
<td width="33%" valign="top">

**`03` · Sistemas & processos**

```diff
+ ERPs e sistemas empresariais
+ Diagnóstico de legados
+ Modernização e integração
+ Automação de processos
```

</td>
</tr>
</table>

<br/>

## `$` stack

<div align="center">

<img src="https://skillicons.dev/icons?i=ts,js,php,python,cs&theme=dark&perline=10" alt="Linguagens" />
<br/>
<img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind,nodejs,nestjs,express,laravel,prisma&theme=dark" alt="Frontend e backend" />
<br/>
<img src="https://skillicons.dev/icons?i=postgres,mysql,supabase,redis,docker,linux,arch,ubuntu,aws,nginx&theme=dark" alt="Dados e infraestrutura" />
<br/>
<img src="https://skillicons.dev/icons?i=git,github,vscode,postman&theme=dark" alt="Ferramentas" />

</div>

<details>
<summary><code>cat stack.yml</code></summary>

<br/>

```yaml
linguagens:     [TypeScript, JavaScript, PHP, Python, C#]
frontend:       [React, Next.js, Vite, Tailwind CSS]
backend:        [Node.js, NestJS, Express, Laravel, Prisma]
dados:          [PostgreSQL, MySQL, MariaDB, Supabase, Redis]
infraestrutura: [Linux (Arch, Ubuntu), Docker, Nginx, AWS]
ia:             [RAG, LangChain, Embeddings, Vector DB, Agentes, Claude, OpenAI]
ferramentas:    [Git, GitHub, VS Code, Postman]
```

</details>

<br/>

## `$` ia aplicada

<div align="center">

<img src="./assets/agents-office.svg" width="100%" alt="Escritório isométrico com agentes de IA trabalhando: RAG, LangChain, Retriever, Expert KB e Code Review" />

<sub><code>agents.office</code> — cada agente é uma etapa real dos fluxos que construo</sub>

</div>

<br/>

Uso de LLMs integrado ao ciclo de desenvolvimento, com escopo definido, indo além do prompt: **RAG**, **orquestração com LangChain** e **bases de conhecimento especialista**.

```bash
$ llm --pipeline
  ├── rag            ingestão, chunking, embeddings, busca vetorial e reranking
  ├── langchain      chains, tools, memória e agentes orquestrados
  ├── expert-kb      fluxos de conhecimento especialista: regras, validação e rastreabilidade
  ├── agentes        assistentes por função, integrados às aplicações via API
  ├── legados        mapeamento de código sem documentação, fluxo e dependências
  ├── prompts        estruturados, versionados e avaliados junto do código
  ├── code-review    análise, correção e refatoração assistidas
  ├── docs           documentação técnica gerada a partir do repositório
  └── automação      rotinas empresariais e fluxos operacionais
```

<details open>
<summary><code>cat fluxo-rag.mmd</code></summary>

<br/>

```mermaid
flowchart LR
    U([Usuário]) --> Q[Query]
    Q --> E[Embedding]
    E --> V[(Vector DB)]
    V --> R[Rerank]
    KB[(Expert KB<br/>regras e conhecimento)] --> R
    R --> P[Prompt + contexto]
    P --> L{{LLM}}
    L --> T[Tools: SQL / APIs]
    T --> L
    L --> A([Resposta com fontes])

    D[Documentos / ERP / Legado] -. ingestão .-> C[Chunking] -. embeddings .-> V

    classDef ai fill:#6C63FF,stroke:#8F88FF,color:#fff
    classDef data fill:#0F1420,stroke:#22D3EE,color:#E6EDF3
    class E,R,L,P ai
    class V,KB,D,C data
```

</details>

<div align="center">

<img src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude" />
<img src="https://img.shields.io/badge/OpenAI-000000?style=flat-square&logo=openai&logoColor=white" alt="OpenAI" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain" />
<img src="https://img.shields.io/badge/RAG-6C63FF?style=flat-square&logo=databricks&logoColor=white" alt="RAG" />
<img src="https://img.shields.io/badge/Vector%20DB-22D3EE?style=flat-square&logo=postgresql&logoColor=0B0E14" alt="Vector DB" />
<img src="https://img.shields.io/badge/Expert%20Knowledge-EC4899?style=flat-square&logo=bookstack&logoColor=white" alt="Expert Knowledge" />
<img src="https://img.shields.io/badge/Agentes%20de%20IA-6C63FF?style=flat-square&logo=probot&logoColor=white" alt="Agentes de IA" />
<img src="https://img.shields.io/badge/Automações%20com%20LLMs-1E293B?style=flat-square&logo=robotframework&logoColor=white" alt="Automações com LLMs" />

</div>

> [!IMPORTANT]
> A IA acelera a escrita. A arquitetura, as decisões e a responsabilidade pelo que vai para produção continuam sendo minhas.

<br/>

## `$` atividade

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=DevMacedojr&show_icons=true&hide_border=true&hide_title=true&theme=transparent&icon_color=6C63FF&text_color=8B95A8&include_all_commits=true&count_private=true&locale=pt-br">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=DevMacedojr&show_icons=true&hide_border=true&hide_title=true&theme=transparent&icon_color=6C63FF&text_color=57606A&include_all_commits=true&count_private=true&locale=pt-br" alt="Estatísticas do GitHub">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=DevMacedojr&layout=compact&hide_border=true&hide_title=true&theme=transparent&text_color=8B95A8&langs_count=6&locale=pt-br">
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DevMacedojr&layout=compact&hide_border=true&hide_title=true&theme=transparent&text_color=57606A&langs_count=6&locale=pt-br" alt="Linguagens mais utilizadas">
</picture>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=DevMacedojr&hide_border=true&background=00000000&ring=6C63FF&fire=22D3EE&currStreakLabel=6C63FF&sideLabels=8B95A8&currStreakNum=E6EDF3&sideNums=E6EDF3&dates=5C6577&locale=pt_BR">
  <img height="150" src="https://streak-stats.demolab.com?user=DevMacedojr&hide_border=true&background=00000000&ring=6C63FF&fire=22D3EE&currStreakLabel=6C63FF&sideLabels=57606A&currStreakNum=0B0E14&sideNums=0B0E14&dates=57606A&locale=pt_BR" alt="Sequência de contribuições">
</picture>

<br/><br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DevMacedojr/DevMacedojr/output/snake-dark.svg">
  <img width="92%" src="https://raw.githubusercontent.com/DevMacedojr/DevMacedojr/output/snake.svg" alt="Contribuições">
</picture>

</div>

<br/>

## `$` contato

<div align="center">

<a href="https://www.linkedin.com/in/ljml200"><img src="https://img.shields.io/badge/LinkedIn-0B0E14?style=for-the-badge&logo=linkedin&logoColor=6C63FF" alt="LinkedIn" /></a>
<a href="mailto:youloiolatube@gmail.com"><img src="https://img.shields.io/badge/E--mail-0B0E14?style=for-the-badge&logo=gmail&logoColor=6C63FF" alt="E-mail" /></a>
<a href="https://github.com/DevMacedojr"><img src="https://img.shields.io/badge/GitHub-0B0E14?style=for-the-badge&logo=github&logoColor=6C63FF" alt="GitHub" /></a>
<a href="https://instagram.com/omacedojose2k25"><img src="https://img.shields.io/badge/Instagram-0B0E14?style=for-the-badge&logo=instagram&logoColor=6C63FF" alt="Instagram" /></a>

<br/><br/>

```console
$ echo $MOTTO
Tecnologia não é apenas escrever código — é entender problemas reais
e transformá-los em soluções escaláveis e funcionais.
```

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6C63FF,100:22D3EE&height=90&section=footer" width="100%" alt="" />

</div>
