# Hey, I'm Sparsh 

Third-year CSE undergrad in India. I build real-time systems and AI products, and
I run a student org that teaches financial literacy to people who never got taught it.

Most of what I build falls into one of two buckets: **things that have to happen
right now** (voice pipelines, live classrooms, order matching) or **things that
should have been taught in school** (money, markets, risk).

---

### What I'm working on

**[Maven AI](https://github.com/sparsh-j01/maven-ai)** — real-time voice mock interviews
Talk to a low-latency interviewer that takes clean turns and asks adaptive follow-ups,
run a live coding round graded against hidden tests, and get back a rubric-scored
report with a replayable transcript.

The interesting part isn't the UI. It's a long-lived stateful voice worker sitting
apart from the serverless web app, a turn-based STT → LLM → TTS loop over
LiveKit/WebRTC, a tool-driven state machine that persists its cursor so an agent
restart resumes where it left off, and a scorer I proved with an eval harness
instead of assuming. Push-to-talk with no barge-in, so pausing mid-answer to think
never cuts you off.

`Next.js 15` · `TypeScript` · `Python` · `LiveKit` · `Postgres/pgvector` · `Inngest`

**[OptiMarket](https://optimarket-psi.vercel.app)** — bond portfolio optimization that runs in your browser
Nelson-Siegel yield curve, SLSQP optimizer, Monte Carlo VaR/CVaR, multi-scenario
stress testing, on real FINRA TRACE data with actual CUSIPs.

The whole SciPy optimizer is compiled to WebAssembly via Pyodide and runs
client-side in a Web Worker. No backend, no cold start, no data leaving your
device, and $0/month to keep online.

`Next.js` · `TypeScript` · `Python` · `Pyodide/WASM` · `SciPy`

**Atlas** *(private)* — live in-class quizzes from your own lecture material
Upload a lecture PDF, AI builds a full editable deck — quiz, polls, word clouds —
then run it live. Students join from their phones with a room code and 100+ of them
answer the same question at the same instant while the leaderboard animates on the
big screen. Mentimeter's visuals, Kahoot's competition, with an AI front door.

`Next.js` · `TypeScript` · `Supabase Realtime` · `Claude API`

**Ledgr** *(early)* — a paper trading platform in Node, TypeScript and Postgres.
Currently deep in matching engine territory, working out how orders rest, cross
and fill before anything gets built on top of them.

**WhatsApp CRM** *(with [@RishvinReddy](https://github.com/RishvinReddy))* — a CRM that
lives inside WhatsApp. Customers hold a normal conversation on Meta's WhatsApp Cloud
API while Gemini handles intent; the business gets a real-time dashboard behind it.
Grocery ordering is just the first vertical — the conversational layer drops onto
any catalogue.

---

### Outside the terminal

I'm **President of Finance Studio**, a student org teaching financial literacy to
economically disadvantaged communities. We cover the basics that actually compound —
budgeting, saving, credit, how debt really works — for people who were never given
access to any of it.

I also built a
[bilingual financial literacy chatbot](https://github.com/sparsh-j01/financial-literacy-chatbot)
on Gemini so the material is reachable in more than one language, and outside
session hours.

---

### Tools I reach for

**Languages** TypeScript · Python · JavaScript · Java

**Frontend** Next.js · React · Tailwind

**Backend** Node.js · FastAPI · Express · LiveKit · Inngest

**Data** PostgreSQL · pgvector · Supabase · Redis · MongoDB · Prisma

**AI** Claude API · Gemini · RAG · agent tooling

**Infra** Docker · Kubernetes · AWS · Vercel · Cloudflare · GitHub Actions

---

### Currently

- Building the Ledgr matching engine
- Trying to make LLMs do work that survives contact with production

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/sparsh-jhunjhunwala/) ·
[X](https://x.com/sparsh_jjwala) ·
[sparshjjwala.work@gmail.com](mailto:sparshjjwala.work@gmail.com)
