## Jérémie Goldberg

Platform & cloud architect, Montpellier. Twenty years in operations — I started
as a systems administrator, was called DevOps, then architect, then platform.
Same job throughout: **make production hold, and stay out of the way of the
people who keep it alive.**

Currently at [Kaliop](https://www.kaliop.com), working with clients at very
different levels of technical maturity — sometimes from scratch, sometimes
taking over an existing platform, sometimes just helping a team modernise
without breaking what already works.

Before that, four years building the DevOps foundations of
[Tezos](https://tezos.com) at Nomadic Labs: infrastructure as code from nothing,
CI that had to scale on demand, and a public snapshot service that saved
strangers several days of waiting.

**AWS · GCP · Azure · Scaleway · Kubernetes · Terraform / OpenTofu · GitLab CI · Go**

---

### I write about this

Code shows what I built. The blog shows how I decide — which is usually the more
useful half. Everything is published in French and English at
**[blog.jeremiegoldberg.com](https://blog.jeremiegoldberg.com)**.

A few that make the argument better than a CV would:

- **[Nobody should run apply from a laptop](https://blog.jeremiegoldberg.com/en/blogs/nobody-should-run-apply-from-a-laptop/)**
  — as long as infrastructure as code is applied from workstations, your
  repository doesn't describe your production. It describes what somebody had on
  their disk the day it worked.
- **[The technical debt nobody sees](https://blog.jeremiegoldberg.com/en/blogs/the-technical-debt-nobody-sees/)**
  — code debt gets a ticket. Infrastructure debt has no file, no review, no line
  on the invoice. It lives in what was never done.
- **[We didn't break the silo, we moved it](https://blog.jeremiegoldberg.com/en/blogs/we-didnt-break-the-silo-we-moved-it/)**
  — a platform team that becomes indispensable has failed. The goal is that other
  teams stop needing you for the ordinary things.
- **[Sovereign means nothing. Reversible does.](https://blog.jeremiegoldberg.com/en/blogs/sovereign-means-nothing-reversible-does/)**
  — sovereignty is declared and can't be verified. Reversibility is a number:
  how long, and how much, to leave.
- **[Your AI has no version number](https://blog.jeremiegoldberg.com/en/blogs/your-ai-has-no-version-number/)**
  — we spent fifteen years making everything reproducible, then wired a
  non-deterministic dependency into production without a single meeting about it.
- **[Being right is not enough](https://blog.jeremiegoldberg.com/en/blogs/being-right-is-not-enough/)**
  — on the transformations that don't take, the teams that aren't ready, and the
  two or three people you leave behind.

---

### Worth a look here

**Tools I built because I needed them**

| | |
|---|---|
| **[self-documenting-wiki](https://github.com/jeremiegoldberg/self-documenting-wiki)** | Generates a documentation index from repository descriptions and topics. Go, standard library only. Documentation that can't drift, because nothing about it is written by hand. |
| **[kc2tf](https://github.com/jeremiegoldberg/kc2tf)** | Exports a running Keycloak realm into importable Terraform. |
| **[gitlab-cli](https://github.com/jeremiegoldberg/gitlab-cli)** | Go CLI for GitLab merge requests, with changelog validation and merge blocking. |
| **[web-lang-detector](https://github.com/jeremiegoldberg/web-lang-detector)** | Detects the language and country of a web page from its markup, headers and TLD. |

**Small services, deployed end to end**

The three below share one Terraform module: a deployment, a service, and a
namespace, called once per instance. Two Python APIs and a Go bot go through the
same paved road — which is the point of a paved road.

| | |
|---|---|
| **[flair-ner-api](https://github.com/jeremiegoldberg/flair-ner-api)** | Named entity recognition behind an HTTP API. One model per instance, four languages from the same module. GPU scheduling, CPU fallback. |
| **[google-news-decoder-api](https://github.com/jeremiegoldberg/google-news-decoder-api)** | Resolves obfuscated Google News URLs back to the publisher's address. |
| **[discordquizbot](https://github.com/jeremiegoldberg/discordquizbot)** | Quiz bot for Discord in Go. Stateful, which makes it more interesting to operate than an API. |
| **[dify-terraform](https://github.com/jeremiegoldberg/dify-terraform)** | Deploying an LLM application platform on Kubernetes, described end to end. |

**Kept as a record**

| | |
|---|---|
| **[dcos-scaleway](https://github.com/jeremiegoldberg/dcos-scaleway)** | A seven-node DC/OS cluster on Scaleway, from 2018. What orchestration looked like before Kubernetes won. |
| **[terraform_howto](https://github.com/jeremiegoldberg/terraform_howto)** · **[docker_howto](https://github.com/jeremiegoldberg/docker_howto)** | Companions to blog posts. Small on purpose. |

Every README says what the project does *and what it is missing* — no ingress,
no resource limits, no readiness probe, an in-memory scoreboard. If something
here would not survive production, it says so.

---|---|
| **[self-documenting-wiki](https://github.com/jeremiegoldberg/self-documenting-wiki)** | Generates a documentation index from repository descriptions and topics. Go, standard library only. Documentation that can't drift, because nothing about it is written by hand. |
| **[kc2tf](https://github.com/jeremiegoldberg/kc2tf)** | Exports a running Keycloak realm into importable Terraform. |
| **[gitlab-cli](https://github.com/jeremiegoldberg/gitlab-cli)** | Go CLI for GitLab merge requests, with changelog validation and merge blocking. |
| **[dify-terraform](https://github.com/jeremiegoldberg/dify-terraform)** | Deploying an LLM application platform on Kubernetes, described end to end. |
| **[dcos-scaleway](https://github.com/jeremiegoldberg/dcos-scaleway)** | A seven-node DC/OS cluster on Scaleway, from 2018. Kept as a record of what orchestration looked like before Kubernetes won. |

The older repositories are teaching material, most of them companions to blog
posts. They are small on purpose.

---

[Blog](https://blog.jeremiegoldberg.com) · [LinkedIn](https://www.linkedin.com/in/jeremiegoldberg/)
