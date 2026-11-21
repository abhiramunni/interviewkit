# InterviewKit — Walk In Ready: Network Engineer Interview Prep

Sixty questions a real interviewer asks — CCNA fundamentals, routing and switching, FortiGate security, troubleshooting, and the HR round — each with a plain-words model answer. Mark what you know, drill what you don't, then sit a timed mock before the day.

Live: **https://abhiramunni.github.io/interviewkit/**
Published: 21 Nov 2026

## What it does

- **Interview card + live countdown** — Set your role, company and interview date. A ticking countdown (days / hours / minutes / seconds) follows it, and the checklist and summary use it too.
- **Readiness dashboard** — An honest readiness ring that only counts questions you marked "I know this", per-topic progress bars, and your weakest topic called out by name.
- **Five topic cards** — Networking Basics, Routing & Switching, Security & FortiGate, Troubleshooting, HR & Behavioural. Tap a card to open its questions.
- **Question deck (60 questions)** — Every question carries a model answer written in plain words and a "remember this" one-liner. Filter by topic, review-only, or not-yet-marked. Flashcard mode hides the answers until you tap.
- **Rapid-fire drill** — 60 seconds, random questions, grade yourself honestly. Best score is saved on-device.
- **Timed mock interview** — 10 questions, two from each topic, two minutes per question with a countdown bar. Self-grade each answer; the result screen gives a verdict, your weakest topic, and a "revise next" list. Shaky answers are auto-marked for review.
- **Subnet lab** — Type any IP and prefix; network, broadcast, usable range, host count, mask and wildcard appear instantly. Six one-tap examples (/8 to /30) included.
- **STAR answer builder** — Situation / Task / Action / Result boxes turn your stories into copy-ready behavioural answers. Save as many as you like.
- **Interview-day checklist** — 12 items across "the day before" and "interview day", with a progress percentage.
- **Six plain-language guides** — The STAR method, subnetting in 60 seconds, "tell me about yourself", salary talk for freshers, what to ask the interviewer, and after the interview.
- **Your data stays yours** — Everything is saved in localStorage on your device. Nothing is uploaded. Copy a one-paragraph prep summary, remove the samples, or erase everything with two taps.

## The content (hand-checked)

- 60 questions: 12 per topic. Technical answers verified against CCNA-level networking: OSI layers, TCP vs UDP, DORA, ARP, VLANs, STP, OSPF cost, AD values (connected 0, static 1, EIGRP 90, OSPF 110, RIP 120), FortiGate first-match policies, SNAT/DNAT, SD-WAN.
- Subnet maths: 192.168.1.10/24 → network 192.168.1.0, broadcast 192.168.1.255, 254 hosts, range .1–.254. 10.0.0.5/8 → 16,777,214 hosts. 192.168.10.77/26 → network .64, broadcast .127, 62 hosts. 10.10.10.10/30 → network .8, broadcast .11, 2 hosts.
- Mock interview: 10 questions, 2 per topic, 120 seconds each.
- Drill: 60 seconds, random questions, best score persisted.

## Tech

- One single self-contained `index.html` — no backend, no signup, no build step.
- Two AI-generated warm-editorial photos (interview desk hero, preparation flat-lay). In this repo they are separate files (`interviewkit-hero.webp`, `interviewkit-flatlay.webp`) referenced by `index.html`; the local build embeds them as base64 for QA.
- Fraunces + Inter, warm editorial palette (ivory paper, espresso ink, bronze, amber, terracotta).
- Cinematic intro (4s, tap-to-skip, quick on return visits) and a 3-step onboarding tour.
- QA: headless jsdom assertions (`qa-test.js`), `node --check`, zero uncaught JS errors.
