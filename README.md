<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=190&section=header&text=Pedro%20Santos&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Informatics%20and%20Computing%20Engineering%20%C2%B7%20FEUP&descAlignY=58&descSize=18" alt="Pedro Santos" />

### Hi, I'm Pedro 👋

**Final-year student of Informatics and Computing Engineering (L.EIC) at FEUP** · Porto, Portugal

I build things close to the metal and on the web — from network protocols in C to full-stack applications in Laravel. This page is my portfolio: the projects below are coursework I'm proud of, documented and open to explore.

[![GitHub](https://img.shields.io/badge/GitHub-putridpunk-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/putridpunk)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Pedro%20Santos-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pedro-simas-santos-30a105280/)
[![FEUP](https://img.shields.io/badge/FEUP-L.EIC-7A003C?style=for-the-badge)](https://sigarra.up.pt/feup/en/CUR_GERAL.CUR_VIEW?pv_curso_id=22841)
[![Location](https://img.shields.io/badge/Porto-Portugal-2c5364?style=for-the-badge&logo=googlemaps&logoColor=white)](#)

</div>

---

## About me

I'm in my final year of the **Bachelor in Informatics and Computing Engineering (L.EIC)** at the **Faculty of Engineering of the University of Porto (FEUP)**, interested in the layers that make software work: protocols, operating systems, databases and the interfaces people actually use.

My coursework has taken me from **HDLC-style framing and reliable transfer over a serial link in C**, through **parser combinators and truth tables in Haskell**, to a **Laravel + PostgreSQL web platform** and a **user-centred public-services project**. I like code that is correct under failure, documentation that explains *why*, and interfaces that don't make people think.

- 🎓 **Education:** Bachelor in Informatics and Computing Engineering (L.EIC), FEUP — 2026/2027
- 💼 **Open to:** internships and junior software engineering roles
- 🧠 **Currently deepening:** backend engineering, networking and application security
- 📍 **Based in:** Vila Nova de Gaia / Porto, Portugal

---

## Tech stack

**Languages**

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5D4F85?style=flat-square&logo=haskell&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Frameworks & data**

![Laravel](https://img.shields.io/badge/Laravel%2012-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Blade](https://img.shields.io/badge/Blade-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%2016-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Eloquent](https://img.shields.io/badge/Eloquent-FF2D20?style=flat-square&logo=laravel&logoColor=white)

**Tools & environments**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![WSL](https://img.shields.io/badge/WSL-4D4D4D?style=flat-square&logo=windows&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

**Concepts**

`Computer networks` · `Protocol design` · `Operating systems` · `Application security` · `Relational databases & SQL` · `Web application architecture` · `Human–computer interaction` · `Functional programming` · `Parsing` · `Technical writing`

---

## Featured projects

### 📡 RCOM — Reliable file transfer over a serial link

> A full link-layer and application-layer protocol in C, built on top of a provided serial-port API.

Implemented an **HDLC-style framing** protocol with byte stuffing, **BCC1/BCC2** error detection, **stop-and-wait ARQ** with alternating sequence numbers, `RR`/`REJ` acknowledgements, `SET`/`UA`/`DISC` connection management, and `SIGALRM`-driven timeouts and retransmissions. On top of it, a simple application protocol with `START`/`DATA`/`END` packets and TLVs for file name and size.

Validated with a virtual cable under **injected bit errors, propagation delay, and link disconnections** — the received file stays byte-identical to the original. The project also reports throughput and protocol efficiency.

**Course:** Redes de Computadores (RC) — Computer Networks · 3rd year, 6 ECTS<br/>
**Stack:** `C` · `Linux/WSL` · `termios` · `socat` · `Make`<br/>
**Repo:** [github.com/putridpunk/RCOM](https://github.com/putridpunk/RCOM)

<br/>

### 🧮 PFL — Propositional logic classifier

> A parser and truth-table engine for propositional logic, written in Haskell.

Built with **parser combinators**: `prop` and `term` handle operator precedence and associativity, `factor` dispatches on negation, parentheses, constants and variables, and the parser only accepts input that consumes the whole line. The classifier generates all `2^n` truth assignments and labels each proposition as `TAUTOLOGY`, `CONTRADICTION` or `CONTINGENT`, with an `INVALID` fallback.

Backed by a **65-case test suite** plus whitespace edge cases.

**Course:** Programação Funcional e em Lógica (PFL) — Functional and Logic Programming · 3rd year, 6 ECTS<br/>
**Stack:** `Haskell` · `GHC` · parser combinators · recursion<br/>
**Repo:** [github.com/putridpunk/PFL-project-1](https://github.com/putridpunk/PFL-project-1)

<br/>

### 🗂️ LBAW — Collaborative project management platform

> A team-based web application for organising projects, tasks and communication.

Built on a **Laravel 12 / PHP 8.3 / PostgreSQL 16** stack with Blade and vanilla JavaScript. The domain model covers accounts and roles (`Coordinator` / `Member`), projects, tasks with status and priority, comments and a forum, attachments, time logging, invitations and notifications.

The database is designed directly in SQL with **enums, constraints and triggers**, and the application enforces **policy-based authorization** on every protected resource, server-side validation, CSRF protection and escaped output. Work in progress as a course project.

**Course:** Laboratório de Bases de Dados e Aplicações Web (LBAW) — Databases and Web Applications Laboratory · 3rd year, 6 ECTS<br/>
**Stack:** `PHP` · `Laravel` · `PostgreSQL` · `Blade` · `Docker`<br/>
**Repo:** academic GitLab repository — available on request

<br/>

### 🧑‍💻 IPC — "Procedimentos FEUP" public-services app

> A user-centred redesign of how FEUP students find and follow administrative procedures.

Four-person HCI project following a **user-centred design process**. We ran an online questionnaire, built a **PACT analysis**, two personas and activity scenarios, then derived functionalities and user stories. The current iteration covers **wireflows, a low-fidelity prototype and usability requirements**, leading into a high-fidelity prototype and user evaluation.

The core finding: the information exists, but students can't find it or understand it — Sigarra is dispersed, opaque after submission, and awkward on mobile.

**Course:** Interação Pessoa-Computador (IPC) — Human–Computer Interaction · 3rd year, 4.5 ECTS<br/>
**Stack:** user research · PACT · wireframing · prototyping · usability evaluation<br/>
**Deliverables:** presentation and report (Portuguese)

<br/>

### 🔐 FSI — SEED security labs

> Hands-on exploitation and mitigation exercises on Linux and web applications.

- **Set-UID & environment variables:** analysed how `fork`, `execve`, `system` and `PATH` interact in privileged programs; exploited a `PATH` hijack against a Set-UID root binary, and demonstrated why invoking a shell from privileged code is dangerous.
- **Web security:** performed stored **XSS** attacks on the Elgg social network, stole session cookies with a `netcat` listener, and wrote a self-propagating **friend-request worm** — then analysed the corresponding mitigations.

**Course:** Fundamentos de Segurança Informática (FSI) — Foundations of Computer Security · 3rd year, 6 ECTS<br/>
**Stack:** `Linux` · `C` · `Bash` · `JavaScript` · `SEED Labs`<br/>
**Deliverables:** lab logs and exploitation write-ups

---

## GitHub in numbers

<div align="center">

<img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=putridpunk&theme=tokyonight" alt="Pedro's GitHub stats" />
<img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=putridpunk&theme=tokyonight" alt="Repositories per language" />

<br/>

<img src="https://streak-stats.demolab.com?user=putridpunk&theme=tokyonight&hide_border=true" alt="GitHub streak" />

</div>

---

## Education

**Faculty of Engineering, University of Porto (FEUP)** — Porto, Portugal<br/>
**Bachelor in Informatics and Computing Engineering (L.EIC)** · 2026/2027 (final year)

A 3-year, 180-ECTS first-cycle degree offered jointly by **FEUP** and the **Faculty of Sciences of the University of Porto (FCUP)**.

**Coursework (3rd year, 1st semester)**

- **Redes de Computadores (RC)** — Computer Networks
- **Laboratório de Bases de Dados e Aplicações Web (LBAW)** — Databases and Web Applications Laboratory
- **Fundamentos de Segurança Informática (FSI)** — Foundations of Computer Security
- **Programação Funcional e em Lógica (PFL)** — Functional and Logic Programming
- **Interação Pessoa-Computador (IPC)** — Human–Computer Interaction

Earlier coursework includes programming fundamentals, discrete mathematics, computer systems fundamentals, algorithms and data structures.

---

## Let's talk

I'm looking for an internship or junior role where I can work on backend systems, infrastructure, AI or security — and keep learning from people who care about doing it properly.

[![LinkedIn](https://img.shields.io/badge/Connect%20on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pedro-simas-santos-30a105280/)
[![GitHub](https://img.shields.io/badge/Follow-putridpunk-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/putridpunk)

<div align="center">

<sub>Thanks for stopping by — feel free to explore the repositories above.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=110&section=footer" alt="" />

</div>
