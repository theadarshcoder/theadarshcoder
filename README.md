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
┌── Key Performance & Engineering Metrics ─────────────────────────────────────────┐
│  • Matching Engine Throughput : ~266,000 orders/sec (P99 execution latency < 18µs) │
│  • Order Book Queue Model     : O(1) Doubly-Linked FIFO Price Level Queues         │
│  • Crash Recovery Test Suite  : 309 / 309 Passing (Deterministic State Replay)     │
│  • Open Source Contributions  : pgmpy (Causal Inference & Probabilistic AI Models) │
└──────────────────────────────────────────────────────────────────────────────────┘
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:64ffda,50:38bdf8,100:818cf8&height=2&section=header" width="100%" alt="divider" />

### Currently Building

| Project | Status | Description |
| :--- | :---: | :--- |
| **[Trading Simulator & Matching Engine](https://github.com/theadarshcoder)** | `Active` | Scaling L2 order-book throughput and building a cross-platform React Native client. |
| **[Avsar](https://github.com/theadarshcoder/Avsar)** | `In Progress` | Transitioning cancellation recovery from hackathon prototype to multi-tenant production SaaS. |

<br>

### Engineering Case Study: Deterministic Crash Recovery in Order Matching

**System:** In-Memory Limit Order Book & Matching Engine (`TypeScript`, `Node.js`, `PostgreSQL`)

* **Problem:** Under simulated server crashes, a naive restart dropped in-flight fills or double-counted settled trades when replaying the event log from disk.
* **Objective:** Guarantee that replaying the log after a crash reconstructs the exact pre-crash account state and satisfies global balance conservation.
* **Implementation:**
  * Added an append-only `account_adjustments` ledger to persist every credit, debit, and fill event atomically.
  * Re-architected boot recovery to route replayed log events directly through the core matching pipeline instead of a separate reconciliation script.
  * Wrote an invariant fuzzer that verifies total cash and total shares remain constant across random process termination points.
* **Outcome:** Validated crash recovery across child-process test harnesses (309 passing tests). Fixed a benchmarking harness defect that masked true execution throughput, correcting measured performance from ~1,767 orders/sec to **~266,000 orders/sec** across 8 concurrent accounts.

<br>

### Featured Projects

#### **[High-Throughput Order Matching Engine & Trading Simulator](https://github.com/theadarshcoder)**
*Deterministic in-memory FIFO limit order book and real-time simulator.*  
`TypeScript` · `Node.js` · `PostgreSQL` · `WebSockets`
* Benchmarked at **~266,000 orders/sec** with sub-20µs execution latency.
* Implemented **$O(1)$** price-level queues using doubly linked lists for instant order entry and cancellation.
* Batched asynchronous ledger persistence to PostgreSQL to keep disk I/O off the critical matching path.

<br>

#### **[Avsar — Appointment Cancellation Recovery SaaS](https://github.com/theadarshcoder/Avsar)**
*Automated slot-recovery system for appointment-driven businesses.*  
`FastAPI` · `MongoDB (Motor)` · `React 18` · `Razorpay` · `Meta Cloud API`
* Broadcasts cancellation openings to waitlisted clients via WhatsApp Cloud API.
* Implements atomic MongoDB reservation locks (`find_one_and_update`) to prevent concurrent double-booking.
* Reconciles Razorpay payment webhooks with cryptographic HMAC SHA-256 signatures.

<br>

#### **[Vision — Remote Exam Proctoring Platform](https://github.com/theadarshcoder/Ai-secure-exam-browser)**
*Online assessment environment with real-time proctoring and code execution.*  
`React` · `TailwindCSS` · `Framer Motion` · `Socket.IO` · `Judge0`
* Real-time browser focus tracking and WebSockets stream handling for proctor oversight.
* Integrated Judge0 sandbox API for compiling and executing coding submissions against test suites.
* Context-based theme system supporting seamless dark and light modes.

<br>

#### **[Kerala Mobility Platform](https://github.com/theadarshcoder/kerala-tourism)**
*Civic transit data platform developed for NATPAC (National Transportation Planning and Research Centre).*  
`FastAPI` · `Redis` · `React Native` · `PostGIS` · `DBSCAN`
* Ingestion pipeline using Redis queues to buffer high-frequency GPS pings (30s intervals) from commuter devices.
* Unsupervised DBSCAN spatial clustering for stop detection paired with a Random Forest transport mode classifier.
* React Native mobile client for passive trip logging with rapid 5-second trip verification.

<br>

### Technical Skills

| Domain | Technologies |
| :--- | :--- |
| **Languages** | <img src="https://skillicons.dev/icons?i=python,ts,js,cpp,html,css" height="28" alt="Languages" /> |
| **Frontend & Mobile** | <img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,redux,vite" height="28" alt="Frontend" /> |
| **Backend & Distributed** | <img src="https://skillicons.dev/icons?i=nodejs,fastapi,express" height="28" alt="Backend" /> |
| **Databases & Storage** | <img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,sqlite" height="28" alt="Databases" /> |
| **Tools & Infrastructure** | <img src="https://skillicons.dev/icons?i=docker,git,github,linux,figma,postman" height="28" alt="Tools" /> |

<br>

### Open Source

* **Contributor to [`pgmpy`](https://github.com/pgmpy/pgmpy)** — Python library for Causal Inference and Probabilistic Graphical Models (Bayesian Networks, Dynamic BNs, Structural Equation Models).

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:64ffda,50:38bdf8,100:818cf8&height=2&section=header" width="100%" alt="divider" />

<div align="center">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=theadarshcoder&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" alt="Adarsh's GitHub Stats" />
</div>
