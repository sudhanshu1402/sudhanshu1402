<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0a0c10,100:1a2332&height=120&section=header" width="100%" alt="" />

# Sudhanshu Singh

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&size=16&duration=3000&pause=1200&color=6EA8FE&center=true&vCenter=true&width=560&lines=Backend+Engineer+%40+Testlify;Distributed+Systems+%26+Durable+Execution;Node.js+%2B+TypeScript;Building+systems+that+survive+crashing" alt="Typing SVG" />

Backend Engineer at Testlify. I build distributed systems, authentication infrastructure, and observability tooling in TypeScript and Node.js.

<a href="https://www.linkedin.com/in/sudhanshusingh1402/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://sudhanshu1402.github.io"><img src="https://img.shields.io/badge/Portfolio-0a0c10?style=for-the-badge&logo=githubpages&logoColor=6ea8fe" alt="Portfolio" /></a>
<a href="https://sudhanshu1402.github.io/system-design-portal"><img src="https://img.shields.io/badge/System%20Design-30363d?style=for-the-badge&logo=readthedocs&logoColor=white" alt="System Design Portal" /></a>

</div>

I work mostly on backend infrastructure: job orchestration, B2B authentication, distributed tracing, and LLM workflows. The projects below are backend systems I've designed and built end-to-end. My full project archive lives on [the portfolio site](https://sudhanshu1402.github.io).

> **Open to backend and platform engineering roles.** Best reached on [LinkedIn](https://www.linkedin.com/in/sudhanshusingh1402/).

I care more about a system staying correct after it crashes than about it looking clever before it does — most of what's below is built around that.

## Tech Stack

<div align="center">

**Backend** &nbsp;
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-E0234E?style=flat-square&logo=redis&logoColor=white)

**Data & Infra** &nbsp;
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**Observability & Cloud** &nbsp;
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

**AI / LLM** &nbsp;
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

</div>

## Featured Systems

| Project | What it does |
| :--- | :--- |
| **[distributed-queue-engine](https://github.com/sudhanshu1402/distributed-queue-engine)** | Redis-backed job processing with priority queuing, exponential backoff, and horizontal worker scaling via BullMQ. |
| **[enterprise-auth-stack](https://github.com/sudhanshu1402/enterprise-auth-stack)** | B2B SSO gateway with SAML 2.0 and SCIM 2.0 provisioning, multi-tenant isolation, and AWS Secrets Manager. |
| **[otel-sdk-node](https://github.com/sudhanshu1402/otel-sdk-node)** | OpenTelemetry wrapper for Node.js: OTLP/gRPC trace and metric export with Pino structured logging. |
| **[multi-region-mongo-patterns](https://github.com/sudhanshu1402/multi-region-mongo-patterns)** | MongoDB Atlas zone-sharding patterns for regional data residency with region-aware writes. |
| **[llm-assessment-pipeline](https://github.com/sudhanshu1402/llm-assessment-pipeline)** | LLM orchestration with dual-model fallback (GPT-4o and Gemini) and Zod-validated structured output. |
| **[system-design-portal](https://github.com/sudhanshu1402/system-design-portal)** | Architecture write-ups with Mermaid diagrams for each system above. |

Full archive and live portfolio: [sudhanshu1402.github.io](https://sudhanshu1402.github.io)

## Open Source

Published packages, not portfolio demos — real users, real semver.

| Project | What it does |
| :--- | :--- |
| **[keel](https://github.com/sudhanshu1402/keel)** [![npm](https://img.shields.io/npm/v/%40sudhanshu1402%2Fkeel.svg)](https://www.npmjs.com/package/@sudhanshu1402/keel) | Durable execution for TypeScript: crash-safe step replay with zero runtime dependencies and a local run dashboard. Same idea as Temporal or Vercel Workflow, without the server, database, or build step. |
| **[nocap](https://github.com/sudhanshu1402/nocap)** [![npm](https://img.shields.io/npm/v/%40sudhanshu1402%2Fnocap.svg)](https://www.npmjs.com/package/@sudhanshu1402/nocap) | Plain-English terminal UI for Claude Code: a readable feed of what it's doing and a clear Yes/No gate before anything risky, on top of the same real permission system. |

<div align="center">
<img src="https://raw.githubusercontent.com/sudhanshu1402/keel/main/demo/demo.gif" alt="keel: a run charges a card, crashes, resumes, and ships without charging twice" width="640" />

<sub>keel — run 1 charges a card and crashes, run 2 resumes and ships without re-charging</sub>
</div>

Also built: **[applicant-exporter](https://github.com/sudhanshu1402/linkedin-applicant-exporter)** — an MV3 browser extension for authorized recruiter workflows, exporting candidate data to XLSX/CSV. The interesting part is the network layer: token-bucket rate limiting, bounded concurrency, and exponential backoff with `Retry-After` handling across two different underlying API generations.

## GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=sudhanshu1402&show_icons=true&hide_border=true&theme=tokyonight&icon_color=6ea8fe&title_color=a78bfa" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sudhanshu1402&layout=compact&hide_border=true&theme=tokyonight&title_color=a78bfa&langs_count=8" alt="Top languages" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=sudhanshu1402&bg_color=0a0c10&color=6ea8fe&line=a78bfa&point=ffffff&area=true&hide_border=true" alt="Activity graph" width="100%" />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake.svg" width="100%" />
</picture>

</div>

<div align="center">

[LinkedIn](https://www.linkedin.com/in/sudhanshusingh1402/) &nbsp;|&nbsp; [Portfolio](https://sudhanshu1402.github.io) &nbsp;|&nbsp; [System Design](https://sudhanshu1402.github.io/system-design-portal)

</div>
