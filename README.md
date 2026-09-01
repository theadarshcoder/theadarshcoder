<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a192f,50:112240,100:020c1b&height=200&section=header&text=Adarsh%20Pratap%20Singh&fontSize=42&fontColor=64ffda&animation=fadeIn&fontAlignY=38" width="100%" alt="Adarsh Pratap Singh" />

  <a href="https://github.com/theadarshcoder">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=3000&pause=1000&color=64FFDA&center=true&vCenter=true&width=750&lines=Systems+%26+Full-Stack+Engineer+%C2%B7+Contributor+%40+pgmpy+%C2%B7+Founder" alt="Tagline" />
  </a>

  <p align="center">
    <a href="https://linkedin.com/in/adarsh-pratap-singh-912539331"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
    <a href="mailto:adarshexclusivemain@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>&nbsp;
    <a href="https://leetcode.com/u/Adarshpratapsingh"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode" /></a>&nbsp;
    <a href="https://github.com/theadarshcoder"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  </p>
</div>

```text
┌── ⚡ SYSTEM TELEMETRY & CORE BENCHMARKS ──────────────────────────────────────────┐
│  ▸ Order Matching Throughput : ~266,000 orders/sec (P99 latency < 18µs)          │
│  ▸ Memory Architecture       : O(1) Doubly-Linked FIFO Price-Level Queues        │
│  ▸ State Replay Invariance   : 309 / 309 Passing (Zero Drift Crash-Safe Ledger)  │
│  ▸ Open Source Upstream      : pgmpy (Causal AI & Probabilistic Graphical Models)│
└──────────────────────────────────────────────────────────────────────────────────┘
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:64ffda,50:38bdf8,100:818cf8&height=2&section=header" width="100%" alt="divider" />

### 🔭 Currently Building

| Project | Status | Focus & Architecture |
| :--- | :---: | :--- |
| 🏦 **[Trading Simulator & Matching Engine](https://github.com/theadarshcoder)** | `🟢 ACTIVE` | Scaling L2 order-book throughput · building cross-platform React Native client |
| 🦷 **[Avsar](https://github.com/theadarshcoder/Avsar)** | `🟡 IN PROGRESS` | Hackathon MVP → multi-tenant production SaaS (WhatsApp queues + Razorpay) |

<br>

### 🧩 Engineering Challenge — Crash-Safe Order Matching at Scale

> **Context:** High-throughput in-memory order matching engine (`TypeScript`, `Node.js`, `PostgreSQL`).

* **Situation:** The trading simulator's in-memory matching engine needed to survive sudden process crashes without corrupting ledger balances or share holdings — a naive restart could silently double-credit or drop trades during state restoration.
* **Task:** Guarantee that replaying the event log after an unexpected crash reproduces the exact deterministic account state as before the crash at production throughput.
* **Action:** 
  * Architected an immutable `account_adjustments` ledger capturing every discrete balance delta alongside order lifecycle events.
  * Replayed engine boot state through the exact same live code paths used during normal trading execution.
  * Implemented an automated conservation fuzzer test asserting total cash and total shares stay invariant after every single transaction.
* **Result:** Verified durable replay via real child-process tests (not mocks), pushed the test suite to **309 passing tests**, and resolved a benchmarking bottleneck — correcting verified throughput from **~1,767 orders/sec** to **~266,000 orders/sec** across 8 concurrent accounts.

<br>

### 🚀 Highlighted Engineering Projects

#### 🏦 **[High-Throughput Order Matching Engine & Trading Simulator](https://github.com/theadarshcoder)**
*Deterministic in-memory FIFO limit order book and real-time simulator, benchmarked against exchange throughput.*
* `TypeScript` · `Node.js` · `PostgreSQL` · `WebSockets`
* ✅ **~266,000 orders/sec** benchmarked throughput with sub-20µs execution latency
* ✅ **$O(1)$** doubly-linked price level queues for instant insertion and cancellation
* ✅ Batched asynchronous ledger persistence to PostgreSQL WAL

<br>

#### 🦷 **[Avsar — Cancellation-Recovery SaaS](https://github.com/theadarshcoder/Avsar)**
*Automated revenue-recovery engine for appointment-driven businesses.*
* `FastAPI` · `MongoDB (Motor)` · `React 18` · `Razorpay` · `Meta Cloud API`
* ✅ Automates last-minute cancellation broadcasts over WhatsApp Cloud API
* ✅ Atomic slot reservation guards — zero double-booking under high concurrency
* ✅ Asynchronous webhook payment verification with cryptographic HMAC SHA-256 signatures

<br>

#### 👁️ **[Vision — AI Exam Governance & Proctoring Platform](https://github.com/theadarshcoder/Ai-secure-exam-browser)**
*Enterprise-grade, high-integrity remote examination environment.*
* `React` · `TailwindCSS` · `Framer Motion` · `Socket.IO` · `Judge0`
* ✅ Full dark/light theming architecture via Context provider with zero layout shift
* ✅ Delivered institutional demo flow, client-side gaze monitoring, and isolated sandbox grading

<br>

#### 🚍 **[Kerala Mobility — Civic Travel Intelligence (NATPAC)](https://github.com/theadarshcoder/kerala-tourism)**
*Civic transit intelligence & passive mobility analytics platform for the National Transportation Planning and Research Centre.*
* `FastAPI` · `Redis` · `React Native` · `PostGIS` · `DBSCAN / ML`
* ✅ Gov-credible visual system designed for state transit planning and modal split analytics
* ✅ Shipped full passive GPS telemetry pipeline and 5-second human-in-the-loop trip verification

<br>

### 🛠️ Tech Stack

| Domain | Stack & Technologies |
| :--- | :--- |
| **Languages** | <img src="https://skillicons.dev/icons?i=python,ts,js,cpp,html,css" height="28" alt="Languages" /> |
| **Frontend & Mobile** | <img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,redux,vite" height="28" alt="Frontend" /> |
| **Backend & Distributed** | <img src="https://skillicons.dev/icons?i=nodejs,fastapi,express" height="28" alt="Backend" /> |
| **Databases & Cache** | <img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,sqlite" height="28" alt="Databases" /> |
| **Tools & Cloud** | <img src="https://skillicons.dev/icons?i=docker,git,github,linux,figma,postman" height="28" alt="Tools" /> |

<br>

### 🌐 Open Source & Research

* **Contributor to [`pgmpy`](https://github.com/pgmpy/pgmpy)** — Python library for Causal AI and Probabilistic Graphical Models (Bayesian Networks, Dynamic BNs, DAGs, Structural Equation Models).

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:64ffda,50:38bdf8,100:818cf8&height=2&section=header" width="100%" alt="divider" />

<div align="center">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=theadarshcoder&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" alt="Adarsh's GitHub Stats" />
</div>
