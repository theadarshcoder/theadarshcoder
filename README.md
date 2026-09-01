<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b192c,100:1e3e62&height=180&section=header&text=Adarsh%20Pratap%20Singh&fontSize=42&fontColor=ffffff&animation=fadeIn" width="100%" alt="Adarsh Pratap Singh" />
  
  <a href="https://github.com/theadarshcoder">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=650&lines=Systems+%26+Full-Stack+Engineer;Open+Source+Contributor+(pgmpy);Founder" alt="Typing Tagline" />
  </a>

  <p align="center">
    <a href="https://www.linkedin.com/in/adarsh-pratap-singh-912539331/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
    <a href="mailto:adarshexclusivemain@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>&nbsp;
    <a href="https://github.com/theadarshcoder"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  </p>
</div>

---

### ⚡ Currently Building

* **[Trading Simulator & Matching Engine](https://github.com/theadarshcoder)** — Scaling the matching engine architecture and building a cross-platform React Native mobile client.
* **[Avsar](https://github.com/theadarshcoder/Avsar)** — Transitioning the cancellation-recovery platform from a hackathon MVP into a multi-tenant production SaaS.

---

### 🚀 Highlighted Projects

* **[High-Throughput Order Matching Engine & Trading Simulator](https://github.com/theadarshcoder)**  
  `TypeScript` · `Node.js` · `PostgreSQL` · `WebSockets`
  - ~266,000 orders/sec benchmarked throughput
  - Sub-20µs execution latency
  - $O(1)$ doubly-linked price level queues
  - Batched async ledger persistence

* **[Avsar — Cancellation-Recovery SaaS](https://github.com/theadarshcoder/Avsar)**  
  `FastAPI` · `MongoDB (Motor)` · `React 18` · `Razorpay` · `Meta Cloud API`
  - WhatsApp cancellation broadcasts
  - Atomic slot reservation guards
  - HMAC SHA-256 webhook verification

* **[Vision — AI Exam Governance & Proctoring Platform](https://github.com/theadarshcoder/Ai-secure-exam-browser)**  
  `React` · `Tailwind` · `Framer Motion`
  - Full dark/light theming architecture via Context provider
  - Institutional demo/pitch delivery

* **[Kerala Mobility — Civic Travel Intelligence for NATPAC](https://github.com/theadarshcoder/kerala-tourism)**  
  `UI/UX` · `Google Stitch` · `React Native` · `FastAPI`
  - Gov-credible visual system
  - Full flow set shipped

---

### 🔬 Engineering Challenge: Crash-Safe Account State Replay

**Context:** [High-Throughput Trading Simulator](https://github.com/theadarshcoder)

* **Situation:** Under process crash and recovery scenarios, a naive sequential restart risked double-crediting balances or dropping trade events during state restoration.
* **Task:** Ensure deterministic, crash-safe replay of account state and strict balance conservation across engine restarts without data corruption.
* **Action:**
  * Implemented an immutable `account_adjustments` ledger to capture discrete balance transitions.
  * Re-architected boot-time state replay to execute through the identical live execution code paths used during active trading.
  * Built a conservation fuzzer test suite to continuously validate balance invariant preservation across simulated crash cycles.
* **Result:** Achieved **309 passing tests** across the test suite with zero state drift. In addition, resolved a benchmarking harness issue, correcting verified throughput from **~1,767 orders/sec** to **~266,000 orders/sec** across 8 concurrent accounts.

---

### 🛠️ Tech Stack

#### Languages
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=ts,js,py,html,css" alt="Languages" />
</a>

#### Frontend
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,redux,vite" alt="Frontend" />
</a>

#### Backend
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=nodejs,express,fastapi" alt="Backend" />
</a>

#### Databases
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,sqlite" alt="Databases" />
</a>

#### Tools
<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=docker,git,github,linux,figma,postman" alt="Tools" />
</a>

---

### 🌐 Open Source

* **Contributor to [`pgmpy`](https://github.com/pgmpy/pgmpy)** — Python library for Causal AI and Probabilistic Graphical Models (Bayesian Networks, DAGs, Structural Equation Models).

---

<div align="center">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=theadarshcoder&show_icons=true&theme=tokyonight&count_private=true&hide_border=true" alt="Adarsh's GitHub Stats" />
</div>
