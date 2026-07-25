<h1 align="center">Hi, I'm Avinash 👋</h1>
<h3 align="center">I write backend code, break Linux installs, and occasionally sleep</h3>

<p align="center">
  <i>B.Tech CSE (AI & ML) @ VIT Bhopal · Building things people didn't ask for, then documenting them like they did</i>
</p>

<p align="center">
  <a href="https://avinashk47.me"><img src="https://img.shields.io/badge/Portfolio-avinashk47.me-black?style=for-the-badge"></a>
  <a href="https://www.linkedin.com/in/avinashkushwaha47/"><img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin"></a>
  <a href="https://github.com/AvinashK47"><img src="https://img.shields.io/github/followers/AvinashK47?label=Follow&style=for-the-badge&logo=github"></a>
</p>

---

## 🧑‍💻 About Me

I'm a backend-leaning fullstack developer who has spent the last few years convincing computers to do things they were clearly not designed to do. I optimize things nobody profiled, automate things nobody asked to skip, and self-host things a $5 SaaS plan would've handled fine — because paying for infrastructure is for people who don't own a spare VPS and several regrets.

Currently studying AI & ML formally, while my actual day-to-day is queues, sandboxes, and yelling at Docker. Balance.

---

## 🚩 Flagship Project: Exec-D

**A Codeforces-style online judge, built from scratch because apparently "just use an existing judge" was too easy.**

This is the one I'll actually defend in an interview. Full Turborepo monorepo, real distributed-systems problems, real 2 AM debugging sessions:

- **Next.js** frontend talking to an **Express** API, which writes submissions to **Postgres (Prisma + Neon)** and enqueues jobs onto **Redis via BullMQ**
- A **worker process** claims jobs, spins up **Docker containers** to compile and run untrusted user code against test cases — network isolated, resource-capped, no funny business
- Verdicts flow back through the pipeline: `PENDING → RUNNING → ACCEPTED / WRONG_ANSWER / TLE / RUNTIME_ERROR / COMPILATION_ERROR` — basically a tiny bureaucracy for your code's failures
- Deployed on an **Oracle ARM64 VM** via **GitHub Actions + PM2**, because I like my deployments the way I like my sleep schedule: automated, so I don't have to think about it

Also survived a personal gauntlet of monorepo hell: Prisma custom output paths that didn't resolve, Turbo caching env vars into oblivion, a missing `dist/` folder, `tsx` ghosting me in production, and a `JWT_SECRET` that GitHub Actions simply forgot existed. Character-building, allegedly.

**Still in progress**, because real projects don't ship "done" — they ship "good enough to demo, terrifying enough to keep improving": per-testcase result storage, one-container-per-submission execution, an actual code editor instead of a glorified textarea, and security hardening beyond "please don't hack this, I'm one person."

---

## 🛠️ Other Projects (Send Help)

**Offline-First AI Voice Assistant** — A privacy-first PWA that runs a WASM-powered Whisper model client-side, because sending someone's voice to a random API felt like a design flaw, not a feature. Web Workers keep the UI thread responsive while the model does the heavy lifting; Next.js API routes keep the LLM keys away from anyone with DevTools open.

**Real-Time Collaborative Whiteboard** — A custom WebSocket server broadcasting drawing events to a canvas rendering engine, because Figma clones are apparently a rite of passage now.

**ShellShockedJS** — A POSIX-compliant shell, written in Node.js, via the CodeCrafters "Build Your Own Shell" challenge. Custom parser, built-ins, process execution, the works. Yes, I wrote a shell in the language most known for `npm install`ing half the internet. No, I don't see the irony.

---

## ⚙️ Tech Stack

**Languages:** JavaScript/TypeScript, Python, Java, C++

**Backend & Data:** Node.js, Express, FastAPI, PostgreSQL, MongoDB, MySQL, Redis, Prisma, BullMQ, WebSockets

**Frontend:** React, Next.js, Tailwind CSS

**Infra & Tooling:** Docker, AWS (EC2), GitHub Actions, Vercel, Linux, Git

**AI-assisted dev:** Claude Code, Gemini CLI — yes, I use AI tools to build things, and no, that's not a personality flaw, that's called using your tools

---

## 🐧 Linux, Or: How I Learned to Stop Worrying and Love the Chroot

Four years of daily-driving **Arch Linux**, with a stint in **Gentoo** compiling my own kernel because apparently pre-built binaries were too mainstream for me.

Most recent flex: recovered a fully kernel-panicked Arch install — busted `initramfs` after an interrupted `pacman` transaction — via chroot, a `mkinitcpio` rebuild, and reinstalling DKMS nvidia modules from a live USB. Nothing was backed up. Everything was fine. This is not a recommendation, it's a confession.

---

## 📚 Currently Grinding

- Working through **DSA** with a self-built, structured curriculum (skipped arrays and sorting — some fundamentals just aren't for me)
- Competitive programming on **CodeChef**, and ranked **3135 (Global)** in **TCS CodeVita 2025** — not top of the leaderboard, but comfortably ahead of everyone who didn't show up
- Certified by IBM in **Python for Data Science** and **React**, which mostly proves I can follow a syllabus when properly incentivized

---

## 🤝 Let's Connect

<p align="left">
  <a href="mailto:avinash.kushwaha1501@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
  <a href="https://www.linkedin.com/in/avinashkushwaha47/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white">
  </a>
  <a href="https://avinashk47.me">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white">
  </a>
</p>

<p align="center"><i>If it's broken, I probably broke it myself first, on purpose, to see how it works.</i></p>
