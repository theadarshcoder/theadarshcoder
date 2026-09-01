<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=blur&color=0:0f172a,100:1e293b&height=170&section=header&text=Adarsh%20Pratap%20Singh&fontSize=34&fontColor=ffffff&fontAlignY=45" width="100%" alt="Adarsh Pratap Singh" />
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=94A3B8&center=true&vCenter=true&width=600&lines=Systems+%26+Full-Stack+Engineer;Open+Source+Contributor+%40+pgmpy;Founder" alt="Typing Tagline" />
  <br><br>
  <a href="https://linkedin.com/in/adarsh-pratap-singh-912539331"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
  <a href="mailto:adarshexclusivemain@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>&nbsp;
  <a href="https://leetcode.com/u/Adarshpratapsingh"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
</div>

<br>

### 🔭 Currently Building

| Project | Status | Focus |
| :--- | :---: | :--- |
| 🏦 **[Trading Simulator & Matching Engine](https://github.com/theadarshcoder)** | 🟢 Active | Scaling engine architecture · shipping React Native client |
| 🦷 **[Avsar](https://github.com/theadarshcoder/Avsar)** | 🟡 In Progress | Hackathon MVP → multi-tenant production SaaS |

<br>

### 🧩 Engineering Challenge — Order Matching at Scale

* **Situation:** The trading simulator's matching engine needed to survive process crashes without corrupting account balances or share holdings — a naive restart could silently double-credit or drop trades.
* **Task:** Guarantee that replaying the event log after a crash always reproduces the exact same account state as before the crash, at production-realistic throughput.
* **Action:** Built an `account_adjustments` ledger to capture every credit/debit, replayed boot state using the same live code paths as normal trading (not a separate reconciliation script), and added a conservation fuzzer test asserting total cash and total shares stay invariant after every single operation.
* **Result:** Verified durable replay via real child-process tests (not mocks), pushed the full test suite to 309 passing, and later fixed a benchmarking bug that was masking true throughput — corrected measured performance from ~1,767 orders/sec to ~266,000 orders/sec across 8 concurrent accounts.

<br>

### 🚀 Highlighted Engineering Projects

#### 🏦 **[High-Throughput Order Matching Engine & Trading Simulator](https://github.com/theadarshcoder)**
*Deterministic in-memory FIFO limit order book and real-time simulator, benchmarked against real exchange throughput.*

* ✅ **~266,000 orders/sec** benchmarked throughput, sub-20µs execution latency
* ✅ **$O(1)$** doubly-linked price level queues
* ✅ Batched asynchronous ledger persistence

<br>

#### 🦷 **[Avsar — Cancellation-Recovery SaaS](https://github.com/theadarshcoder/Avsar)**
*Automated revenue-recovery engine for appointment-driven businesses.*

* ✅ Automates last-minute cancellation broadcasts over WhatsApp
* ✅ Atomic slot reservation guards — zero double-booking under concurrency
* ✅ Async webhook payment verification with HMAC SHA-256 signatures

<br>

#### 👁️ **[Vision — AI Exam Governance & Proctoring Platform](https://github.com/theadarshcoder/Ai-secure-exam-browser)**
*Enterprise-grade, high-integrity remote examination environment.*

* ✅ Full dark/light theming architecture via Context provider, zero changes to existing components
* ✅ Delivered institutional demo flow and pitch materials

<br>

#### 🚍 **[Kerala Mobility — Civic Travel Intelligence (NATPAC)](https://github.com/theadarshcoder/kerala-tourism)**
*Government-grade travel discovery app with passive trip-data collection.*

* ✅ Gov-credible visual system — deep green + gold, bordered flat cards, no shadows
* ✅ Shipped full flows: Home, Trip Verification, Trip Detail, Privacy Center, Discovery

<br>

### 🛠️ Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | <img src="https://skillicons.dev/icons?i=python,ts,js,cpp" height="28" alt="Languages" /> |
| **Frontend** | <img src="https://skillicons.dev/icons?i=react,tailwind,vite" height="28" alt="Frontend" /> |
| **Backend** | <img src="https://skillicons.dev/icons?i=nodejs,fastapi,express" height="28" alt="Backend" /> |
| **Databases** | <img src="https://skillicons.dev/icons?i=postgres,mongodb" height="28" alt="Databases" /> |
| **Tools** | <img src="https://skillicons.dev/icons?i=git,github,vercel,postman" height="28" alt="Tools" /> |

<br>

### 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=theadarshcoder&show_icons=true&theme=default&hide_border=true&hide_title=true&count_private=true" height="165" alt="Adarsh's GitHub Stats" />
</div>
