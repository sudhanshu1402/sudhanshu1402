<div align="center">

# Sudhanshu Singh

<img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&size=17&duration=3200&pause=1200&color=6EA8FE&center=true&vCenter=true&width=580&lines=Backend+Engineer+%40+Testlify;Distributed+systems+%26+durable+execution;Systems+that+stay+correct+after+they+crash" alt="Backend Engineer at Testlify — distributed systems and durable execution" />

<br />

<a href="https://www.linkedin.com/in/sudhanshusingh1402/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://sudhanshu1402.github.io"><img src="https://img.shields.io/badge/Portfolio-0a0c10?style=for-the-badge&logo=githubpages&logoColor=6ea8fe" alt="Portfolio" /></a>
<a href="https://sudhanshu1402.github.io/system-design-portal"><img src="https://img.shields.io/badge/System%20Design-30363d?style=for-the-badge&logo=readthedocs&logoColor=white" alt="System Design Portal" /></a>
<a href="https://www.npmjs.com/package/@sudhanshu1402/keel"><img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm" /></a>

</div>

---

I build backend infrastructure in TypeScript and Node.js: job orchestration, B2B authentication, distributed tracing, and LLM workflows. I care more about a system staying correct after it crashes than about it looking clever before it does, and most of what's below is built around that.

Currently a Backend Engineer at Testlify. **Open to backend and platform engineering roles** — best reached on [LinkedIn](https://www.linkedin.com/in/sudhanshusingh1402/).

## Tech

| | |
| :-- | :-- |
| **Languages** | ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) |
| **Data** | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![BullMQ](https://img.shields.io/badge/BullMQ-E0234E?style=flat-square&logo=redis&logoColor=white) |
| **Observability** | ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) |
| **AI / LLM** | ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) |

## Spotlight — keel

[![npm](https://img.shields.io/npm/v/%40sudhanshu1402%2Fkeel.svg?style=flat-square&color=CB3837)](https://www.npmjs.com/package/@sudhanshu1402/keel) &nbsp; [![MIT](https://img.shields.io/badge/License-MIT-6ea8fe.svg?style=flat-square)](https://github.com/sudhanshu1402/keel/blob/main/LICENSE) &nbsp; [![zero deps](https://img.shields.io/badge/runtime%20deps-0-brightgreen?style=flat-square)](https://github.com/sudhanshu1402/keel)

**[keel](https://github.com/sudhanshu1402/keel)** is durable execution for TypeScript. You write work as named steps; when a step finishes, keel saves its result, so a run that dies at step 7 restarts at step 7 instead of re-running everything from the top. Same core idea as Temporal or Vercel Workflow, but with no server, no database, and no build step — it runs anywhere plain Node runs.

The clearest way to see it is a crash: run 1 charges a card and dies before shipping, run 2 resumes and ships **without charging the card twice**.

<div align="center">
<img src="https://raw.githubusercontent.com/sudhanshu1402/keel/main/demo/demo.gif" alt="keel: run 1 charges a card and crashes, run 2 resumes and ships without re-charging" width="720" />
</div>

## Systems I've built

Backend systems designed and built end-to-end. Each has a matching architecture write-up on the [system design portal](https://sudhanshu1402.github.io/system-design-portal).

| Project | What it does |
| :-- | :-- |
| **[distributed-queue-engine](https://github.com/sudhanshu1402/distributed-queue-engine)** | Redis-backed job processing: priority queuing, exponential backoff, horizontal worker scaling via BullMQ. |
| **[enterprise-auth-stack](https://github.com/sudhanshu1402/enterprise-auth-stack)** | B2B SSO gateway with SAML 2.0 and SCIM 2.0 provisioning, multi-tenant isolation, per-tenant AWS Secrets Manager. |
| **[otel-sdk-node](https://github.com/sudhanshu1402/otel-sdk-node)** | OpenTelemetry wrapper for Node.js: OTLP/gRPC trace and metric export with Pino structured logging. |
| **[multi-region-mongo-patterns](https://github.com/sudhanshu1402/multi-region-mongo-patterns)** | MongoDB Atlas zone-sharding for regional data residency, with a `{region, tenantId}` shard key that avoids scatter-gather. |
| **[llm-assessment-pipeline](https://github.com/sudhanshu1402/llm-assessment-pipeline)** | LLM orchestration with dual-model fallback (GPT-4o → Gemini) and Zod-validated structured output. |

## Also on npm

| Project | What it does |
| :-- | :-- |
| **[nocap](https://github.com/sudhanshu1402/nocap)** [![npm](https://img.shields.io/npm/v/%40sudhanshu1402%2Fnocap.svg?style=flat-square&color=CB3837)](https://www.npmjs.com/package/@sudhanshu1402/nocap) | A plain-English terminal UI for Claude Code — a readable feed of what it's doing and a clear Yes/No gate before anything risky, on the same real permission system. |
| **[applicant-exporter](https://github.com/sudhanshu1402/linkedin-applicant-exporter)** | MV3 browser extension for authorized recruiter workflows. The interesting part is the network layer: token-bucket rate limiting, bounded concurrency, and exponential backoff with `Retry-After` across two API generations. |

## Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=sudhanshu1402&show_icons=true&hide_border=true&theme=tokyonight&icon_color=6ea8fe&title_color=a78bfa&bg_color=0a0c10" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sudhanshu1402&layout=compact&hide_border=true&theme=tokyonight&title_color=a78bfa&bg_color=0a0c10&langs_count=8" alt="Top languages" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=sudhanshu1402&bg_color=0a0c10&color=6ea8fe&line=a78bfa&point=ffffff&area=true&hide_border=true" alt="Contribution activity graph" width="100%" />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/sudhanshu1402/sudhanshu1402/output/github-contribution-grid-snake.svg" width="100%" />
</picture>

<br /><br />

[LinkedIn](https://www.linkedin.com/in/sudhanshusingh1402/) &nbsp;·&nbsp; [Portfolio](https://sudhanshu1402.github.io) &nbsp;·&nbsp; [System Design](https://sudhanshu1402.github.io/system-design-portal)

</div>
