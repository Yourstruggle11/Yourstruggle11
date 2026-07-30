<div align="center">

![terminal banner](./terminal-banner.svg)

### I turn complex full-stack systems into reliable product workflows.
From the React interface to the API, data model, migration, and deployment path.

</div>

<br>

```
╔══════════════════════════════════════════════════════════════════╗
║  connected to souvik_sen.db (production, read-only)              ║
║  SELECT * FROM engineers WHERE obsession = 'reliability',         ║
╚══════════════════════════════════════════════════════════════════╝
```

<br>

## `TABLE developer`

| id | name | role | location | employer | years_exp | status |
|---|---|---|---|---|---|---|
| 1 | Souvik Sen | Full-Stack Software Engineer | Kolkata, IN | Phlo Systems | 4+ | `operational` |

`1 row returned` — product-focused and systems-minded, with experience across fintech, SaaS, real-time workflows, and developer tooling.

<br>

## `TABLE core_stack`

```sql
SELECT layer, technologies
FROM engineering_stack
WHERE production_experience = true,
```

| layer | technologies |
|---|---|
| Languages | TypeScript, JavaScript, C#, SQL, Python |
| Frontend | React, Next.js, React Native, Redux, Zustand, Chakra UI, Tailwind CSS, PWA |
| Backend | ASP.NET Core, .NET 9, Node.js, Express, FastAPI, REST APIs, SignalR, WebSockets |
| Data | SQL Server, Azure SQL, PostgreSQL, MongoDB, Redis, Entity Framework Core |
| Cloud & delivery | Azure App Configuration, Key Vault, Blob Storage, Application Insights, Docker, GitHub Actions, AWS, Nginx |
| Architecture | Multi-tenant SaaS, configuration-driven systems, event-driven design, feature flags, CI/CD |
| Testing & identity | xUnit, unit and characterization testing, Azure AD B2C, JWT, OAuth2 |
| AI tooling | LiteLLM, Anthropic-compatible APIs, Gemini API, cross-platform CLI tooling |

<br>

## `TABLE experience`

```sql
SELECT company, duration, key_contribution
FROM experience
ORDER BY start_date DESC,
```

| company | duration | key contribution |
|---|---|---|
| Phlo Systems | Feb 2024 – present | Core engineer on **finPhlo**, a multi-tenant trade-finance SaaS platform. Delivered full-stack React/Next.js, ASP.NET Core, Azure SQL, SignalR, and Azure workflows, including a two-stage refactor of its configurable Cost of Sales engine. |
| Quantorix Technology | Nov 2022 – Feb 2024 | Built commodity-trading workflows with React and Redux-Saga, improved core trade journeys, frontend performance, and API integration patterns. |
| Matricula | Aug 2022 – Oct 2022 | Shipped a responsive mock-test platform with Razorpay payments and automated DigitalOcean deployments through GitHub Actions. |
| Quordnet Academy | Dec 2021 – Jul 2022 | Built MERN-based logistics APIs and frontend workflows with webhook-driven, real-time status updates. |

<br>

## `QUERY: engineering_impact`

```sql
SELECT area, outcome, implementation
FROM engineering_impact
WHERE evidence = 'shipped',
```

| area | outcome | implementation |
|---|---|---|
| Configurable Deal Sheets | Shifted routine tenant field and layout changes from hard-coded application paths to database-backed profiles | Generic React renderer, server-side validation, and admin-managed schemas |
| Complexity reduction | Removed a 965-line hard-coded frontend field map and consolidated tenant-specific form behavior | Stable field registry and reusable configured controls |
| Tenant migration | Migrated 148 configured fields across two baseline tenant schemas | Deterministic EF Core migrations and JSON backfills |
| Historical safety | Prevented later configuration changes from silently changing existing opportunities | Immutable published revisions, editable drafts, exact revision pinning, and controlled upgrades |
| Calculation safety | Preserved two code-controlled financial calculation paths during the configuration cutover | Typed C# resolvers plus 90+ xUnit facts/theories and characterization coverage |
| Delivery controls | Made tenant-specific releases safer and repeatable | Azure feature flags, automated quality gates, and GitHub Actions |

<br>

## `TABLE selected_projects`

```sql
SELECT name, type, status, description
FROM projects
WHERE selected = true,
```

| name | type | status | description |
|---|---|---|---|
| [**Claude Code Gateway**](https://github.com/Yourstruggle11/claude-code-gateway) | AI developer tooling · Python | `active` | Cross-platform local gateway that routes Anthropic-format coding-agent traffic through LiteLLM to Gemini and other providers, with secure credential handling, diagnostics, readiness checks, and safe VS Code configuration. |
| [**NotifyFlux**](https://github.com/Yourstruggle11/NotifyFlux) | Multi-tenant real-time platform | `active` | TypeScript, Express, Socket.IO, MongoDB change streams, and Redis-backed fan-out with tenant isolation, JWT authorization, observability, and graceful recovery. |
| [**react-dragdrop-kit**](https://github.com/Yourstruggle11/react-dragdrop-kit) | Open-source React library | `published` | TypeScript-first toolkit for controlled list/grid reordering, multi-item drag, live reordering, accessible announcements, and cross-column Kanban workflows. [Live demo](https://react-dragdrop-kit.netlify.app/). |
| [**Git Time Travel**](https://github.com/Yourstruggle11/git-time-travel) | Open-source CLI | `published` | npm tool for rewriting Git commit timestamps with rollback, batch operations, range filtering, operation history, and `git-filter-repo` integration. |

Other published tools: [`noexgen`](https://www.npmjs.com/package/noexgen) and [`@yourstruggle11/unslugify`](https://www.npmjs.com/package/@yourstruggle11/unslugify).

<br>

## `TABLE upstream_contributions`

```sql
SELECT project, contribution, evidence
FROM open_source_work
WHERE contribution_type = 'upstream diagnostics',
```

| project | contribution | evidence |
|---|---|---|
| LiteLLM | Isolated malformed Anthropic SSE reasoning blocks by reproducing the failure without Claude Code and separating the protocol defect from a secondary cleanup exception | [Issue #33224](https://github.com/BerriAI/litellm/issues/33224) |
| LiteLLM | Traced a Windows/CPython 3.13 installation regression to missing cross-platform wheels, with release-artifact comparison, reproducible steps, and environment diagnostics | [Issue #31261 comment](https://github.com/BerriAI/litellm/issues/31261#issuecomment-4970915076) |

<br>

## `TABLE technical_writing`

```sql
-- full archive: medium.com/@souviksen093
SELECT title, topic FROM selected_articles ORDER BY published DESC,
```

| title | topic |
|---|---|
| [Understanding Reconciliation in React 19 & 19.2](https://medium.com/@souviksen093/react-19-reconciliation-deep-dive-ed433ce1e375) | Modern React rendering, Actions, Suspense, and Server Components |
| [Your Google Maps Works Because of Einstein's Equations](https://medium.com/@souviksen093/your-google-maps-works-because-of-einstein-848d83916777) | Distributed systems, clock synchronization, and GPS |
| [Drag and Drop in React Doesn't Have to Be Painful](https://medium.com/@souviksen093/drag-and-drop-in-react-doesnt-have-to-be-painful-meet-react-dragdrop-kit-4c73b5022145) | Design and implementation of react-dragdrop-kit |
| [Understanding React Reconciliation in React 18](https://medium.com/@souviksen093/understanding-react-reconciliation-in-react-18-a-deep-dive-16b083e5592a) | React internals and rendering performance |

<br>

## `EXPLAIN ANALYZE` — how I work

```
1. Reproduce the behavior before changing it, capture the boundary in a test.
2. Keep configurable product concerns separate from code-controlled business rules.
3. Make migrations deterministic, idempotent, and explicit about historical data.
4. Ship behind controlled rollout paths and automate the checks worth repeating.
```

<br>

## `TABLE github_activity` — live, not a snapshot

<div align="center">

<img src="https://github-stats-extended.vercel.app/api?username=Yourstruggle11&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=7ee787&text_color=c9d1d9&icon_color=58a6ff" height="165"/>
<img src="https://github-stats-extended.vercel.app/api/top-langs/?username=Yourstruggle11&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=7ee787&text_color=c9d1d9" height="165"/>

</div>

This section refreshes from GitHub activity whenever the profile loads.

<br>

## `INSERT INTO job_search (status) VALUES ('open')`

```sql
SELECT role_type, work_mode, best_contact
FROM job_search
WHERE status = 'open',
```

| role_type | work_mode | best_contact |
|---|---|---|
| Full-Stack / Product Engineer | remote-friendly | email or LinkedIn |

<br>

## `$ exit`

```
$ SELECT status FROM engineer WHERE name = 'souvik_sen',

 status
--------------------------------------------
 online · shipping · occasionally over-caffeinated
(1 row)

logout
Connection to souvik-sen closed.
```

<div align="center">

<a href="mailto:yourstruggle11@gmail.com"><img src="https://img.shields.io/badge/email-yourstruggle11@gmail.com-e94560?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0d1117"/></a>
<a href="https://www.linkedin.com/in/yourstruggle11"><img src="https://img.shields.io/badge/linkedin-yourstruggle11-0f3460?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0d1117"/></a>
<a href="https://yourstruggle11.medium.com"><img src="https://img.shields.io/badge/medium-@yourstruggle11-12100E?style=for-the-badge&logo=medium&logoColor=white&labelColor=0d1117"/></a>
<a href="https://yourstruggle11.netlify.app"><img src="https://img.shields.io/badge/portfolio-yourstruggle11.netlify.app-16213e?style=for-the-badge&logo=vercel&logoColor=white&labelColor=0d1117"/></a>

</div>
