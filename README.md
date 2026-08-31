```yaml
# ~/.claude/CLAUDE.md
---
name: André Abreu
role: Tech Lead · Backend & AI Platform Engineering
location: Rio de Janeiro, Brazil (UTC-3)
remote: 10+ years
spoken: [pt-BR (native), en (B2), es (A2), it (A1)]
---
```

## IDENTITY

20+ years in tech. Started in infrastructure — networks, virtualization, storage,
high-availability — then moved to writing the software that runs on top of it.

Today I build AI platforms and the engineering infrastructure that makes
multi-agent code generation reliable enough to actually ship.

## CAPABILITIES

```
ai-platform/*   MCP servers · skills · hooks · subagent orchestration · Agent SDK
                prompt engineering · RAG · embeddings · vector search · evals
backend/*       Go (Fiber, goroutines, worker pools) · REST · gRPC · hexagonal
                PHP (Laravel, Symfony) · microservices · message queuing
infra/*         AWS (ECS, EKS, Lambda, S3) · Terraform · Docker · Kubernetes
                GitHub Actions · GitLab CI · GCP · observability
data/*          PostgreSQL · MySQL · MongoDB/DocumentDB · Redis · Elasticsearch
                DynamoDB · Firestore · indexing and query optimization
```

## CURRENT FOCUS

- **Multi-agent code generation pipelines** — fan-out to specialized agents,
  adversarial verification of every finding before it reaches a human reviewer
- **MCP servers and tool schemas** that expose internal systems to agents
  without handing over the keys
- **Skills, hooks and guardrails as engineering artifacts** — versioned,
  reviewed and tested like any other code, not pasted into a chat window
- **Internal reference for AI-assisted development** — turning what demonstrably
  works into repeatable practice for other engineers
- **Go services in production**, because everything above has to run on something

## OPERATING RULES

```
1. A reported bug becomes a failing test before it becomes a fix.
2. 40 direct lines beat 200 "extensible" ones. Abstraction is earned.
3. Observability before optimization. Measure it before you rewrite it.
4. Plan, execute, document — and only document what someone will read.
5. No deploy without a rollback path.
```

## TRACK RECORD

```
attribution platform · PHP 5 → Go rewrite
  Black Friday transaction loss: 30% (2019) → 0.02% (2020) → effectively zero
  after pod memory tuning. Hexagonal architecture, DocumentDB, Kubernetes on EKS.
  Proposed against initial resistance, prototyped on my own time in five
  languages, chose Go on measured performance. Still running in production today.

unmanned surface vessel · environmental telemetry
  20k+ parallel requests/second from onboard sensor arrays over satellite link.
  Ingestion and delivery of ocean, weather and seabed data to energy majors
  and a federal university.

travel distribution platform · SOAP → REST migration
  Full architectural rewrite of the OTA integration layer under SOLID.
  Then brought in to rescue a second, parallel migration that had stalled.
```

## ALSO IN CONTEXT

```
languages   Python · Ruby · C++ · TypeScript/JavaScript (Node, Vue, Next, React)
practice    SOLID · design patterns · Clean Code · Kanban · Scrum · DevOps
systems     Linux (LPIC 1/2/3 track) · shell automation · legacy maintenance
```

## OFF-DUTY

Girl dad and husband first. Harley rider (H.O.G.), photographer, woodworker.
A fair share of my best debugging happens somewhere between the garage and the road.

## CONTACT

```
linkedin   https://linkedin.com/in/intfrr
github     https://github.com/andreabreu76
```

---

## TELEMETRY

![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=andreabreu76&theme=github_dark)

![](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=andreabreu76&theme=github_dark) ![](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=andreabreu76&theme=github_dark)
