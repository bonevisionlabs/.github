# BoneVision Labs

**Open-source tools for scientific research and cloud deployment.**

We're a digital orthopedics company building AI-powered surgical planning tools. Along the way, we've open-sourced the research infrastructure and deployment templates that power our work.

---

## Projects

| Repo | What It Does | Get Started |
|------|-------------|-------------|
| [**research-agent**](https://github.com/bonevisionlabs/research-agent) | Paper toolkit — statistics, figures, DOCX compilation, and a self-learning feedback loop. Pure Python, zero API calls. | `pip install research-agent` |
| [**claude-research-config**](https://github.com/bonevisionlabs/claude-research-config) | Drop-in `CLAUDE.md` that turns Claude Code into a PhD-level research assistant with workflow protocols, guardrails, and quality standards. | `curl -o CLAUDE.md` [link](https://raw.githubusercontent.com/bonevisionlabs/claude-research-config/main/CLAUDE.md) |
| [**swa-starter**](https://github.com/bonevisionlabs/swa-starter) | Azure Static Web Apps template with 6 security headers, SSO auth (Microsoft/GitHub/Google), CI/CD, and dark/light mode. No build tools needed. | Fork and deploy |

## How They Fit Together

```
claude-research-config (CLAUDE.md)    swa-starter
        │ configures                      │ deploys
        ▼                                 ▼
   Claude Code ◄── calls ──► research-agent    Azure Static Web Apps
   (the brain)               (Python tools)    (the platform)
```

**research-agent** + **claude-research-config** form a complete research pipeline: Claude Code makes all the decisions (what to write, how to frame results, when to retry), while Python functions handle I/O, formatting, and state. No multi-agent overhead, no token cost for tool calls.

**swa-starter** is independent — a production-ready template for shipping secure static sites to Azure.

## Get Started

- **Writing papers?** Install `research-agent`, drop the `CLAUDE.md` into your project, and [start here](https://github.com/bonevisionlabs/claude-research-config#quick-start).
- **Deploying a site?** Fork `swa-starter`, connect Azure, and [push](https://github.com/bonevisionlabs/swa-starter#quick-start).
- **Building research tools?** Check the [research-agent API](https://github.com/bonevisionlabs/research-agent#modules) for stats, figures, and document compilation functions.

---

MIT License | [bonevision.app](https://bonevision.app)
