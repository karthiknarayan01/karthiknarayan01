# Karthik Narayan

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/C++17-00599C?style=flat&logo=cplusplus&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" height="22"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Anthropic%20API-D97757?style=flat&logo=anthropic&logoColor=white" height="22"/>
</p>

---

Software engineer who likes understanding systems from the inside out — how a
database actually executes a query, how a lock-free buffer stays correct under
concurrent access, how an HTTP server behaves with nothing but a `poll()` loop
and no dependencies. I build things to find out, then ship the ones worth
keeping.

---

### What I work on

**Systems fundamentals.**
Concurrency, event loops, and protocols implemented from scratch rather than
taken on faith — a multi-threaded factory floor with a shared buffer and
condition variables, an HTTP server over a raw `poll()` loop with zero
dependencies. The point isn't reinventing the wheel; it's knowing exactly why
the wheel is round.

**AI agents that stay honest.**
Local-first where it matters — an immigration Q&A agent and a personal
assistant that both run entirely on-device via Ollama, no API keys, no data
leaving the machine. And where fidelity is the actual product requirement,
like turning a dense earnings statement into plain language, the hard part
isn't generating fluent text — it's proving the rewrite didn't drop a caveat
or invent a number.

**Shipping finished products, not demos.**
A published iOS app. A full-stack document-simplification product with a
real architecture: client-side PDF extraction, a parallel worker pool,
figures and tables preserved instead of lost in translation. Side projects
that end at a working demo teach less than the last 20% that makes something
actually usable.

**Making the invisible visible.**
A tool that turns a SQL query into a slideshow of what Postgres is actually
doing underneath — parsing, planning, the buffer pool, MVCC, WAL — because
"it's slow, add an index" means a lot more once you've seen why.

---

### Selected projects

**[Plainly](https://github.com/karthiknarayan01/plainly-backend)**
Turns hard-to-read documents — earnings statements, financial filings,
technical books — into plain language without dropping or inventing a single
fact. The PDF is parsed client-side; a pool of backend workers rewrites each
page in parallel; pages with a figure or table are detected from their own
text and shown as the original image alongside the rewrite, so nothing
visual gets silently lost. ([web](https://github.com/karthiknarayan01/plainly-web))

**[pg-internals-visualizer](https://github.com/karthiknarayan01/pg-internals-visualizer)**
Paste a SQL query, get back a slideshow of how PostgreSQL actually executes
it — parsing, planning, lock acquisition, the buffer pool, WAL, MVCC
visibility — reasoned out and diagrammed by Claude, no live database
required. Also proposes one concrete optimization and walks through the
"after" plan.

**[Factory-Simulation](https://github.com/karthiknarayan01/Factory-Simulation)**
A real-time multi-threaded factory floor: part workers manufacture and
deposit into a shared, capacity-limited buffer; product workers assemble
finished goods from exactly the right mix of parts. Access is serialized
with a lock and two condition variables, and every event streams live to a
browser dashboard over Server-Sent Events.

**[HTTP-Linked-List-Server](https://github.com/karthiknarayan01/HTTP-Linked-List-Server)**
A Redis-style in-memory server where each key maps to a linked list of
integers, spoken over a plain HTTP/JSON API. C++17, a `poll()`-based event
loop, and nothing else — no framework, no external dependencies.

**[immigration-assistant](https://github.com/karthiknarayan01/immigration-assistant)**
A US immigration Q&A agent (H1B, F1, B1/B2, L1, EB1–EB3) that separates what
the law says from what tends to happen in practice — enforcement and officer
discretion often diverge from the letter of the law — sourcing documented
real-world cases alongside official guidance. Runs entirely on local
open-source models; no paid API.

---

### Notes on how I work

- If a project only reaches "works on my machine," it's not done — the last
  mile (a real UI, a setup script that actually works, tests that catch
  regressions) is most of the value.
- Local-first by default for anything agent-shaped. A tool that needs a cloud
  API key to run a basic demo has a much higher bar to clear.
- Fidelity beats fluency. A confident-sounding rewrite that quietly drops a
  caveat is worse than an ugly one that keeps it.
- I'd rather implement the primitive once (a lock, an event loop, a linked
  list) than trust it blindly forever after.

*(This section is a first pass based on the shape of my own repos —
edit freely, it's supposed to sound like you.)*

---

### 📊 Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=karthiknarayan01&show_icons=true&hide_border=true&count_private=true"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=karthiknarayan01&layout=compact&hide_border=true"/>
</p>

---

### Elsewhere

Reachable through GitHub — issues and discussions on any of the repositories
above, or the profile inbox.

---

<sub>Opinions here are my own.</sub>
