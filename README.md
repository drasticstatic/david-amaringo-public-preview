# David Amaringo 🌿🎨 — Amazonian Visionary Art

> *A home online for Maestro David Amaringo — Ayahuasca visionary artist, Chaiconi Bari healer, trained by his uncle, the legendary Pablo Cesar Amaringo Shuña, founder of the USKO-AYAR Amazonian School of Painting.*

[![License](https://img.shields.io/badge/license-Private-lightgrey?style=flat)](https://github.com/drasticstatic/david-amaringo) [![Built with Claude Code](https://img.shields.io/badge/Built%20with-Claude%20Code%20CLI-blueviolet)](https://code.claude.com/docs/en/overview) [![Status](https://img.shields.io/badge/Status-%F0%9F%8C%B1%20Early%20Foundation-orange)](https://github.com/drasticstatic/david-amaringo)

---

## Table of Contents

- [David Amaringo 🌿🎨 — Amazonian Visionary Art](#david-amaringo---amazonian-visionary-art)
  - [Table of Contents](#table-of-contents)
  - [🌿 Dearly Beloved](#-dearly-beloved)
  - [🎯 The Goal](#-the-goal)
  - [🏗️ Architecture](#️-architecture)
  - [💻 Development](#-development)
  - [🤝 Collaboration](#-collaboration)
  - [📜 License](#-license)

---

<a id="dearly-beloved"></a>
## 🌿 Dearly Beloved

Maestro David Amaringo is co-founder of Chaiconi Bari. He is a master Ayahuasca visionary artist trained by his uncle, the legendary ayahuasquero curandero visionary artist Pablo Cesar Amaringo Shuña. He has been drinking Ayahuasca for many years, and tells us the plant has taught him to paint just as much as his uncle did — and demands just as much honesty.

He began his training when he was just 14 years old at the "USKO-AYAR" (a Quechua term meaning "Spiritual Prince" or "Wise Prince") Amazonian School of Painting co-founded by Pablo. He teaches there to this day. There, he studied spiritual principles and the art of "Well-Living" through painting as well as the English language. His work has been displayed in galleries worldwide, including the Museum of Children's Art in Oslo, Norway, where it remains permanently on exhibition.

Aside from his work with his uncle, he has trained with the people of the Shipibo tradition for many years and continues to do so. He is an exceptional guide of the upper Amazon basin, a skilled English translator, and a masterful ceremonial facilitator — teaching in Ayahuasca Artisan Workshops and serving as lead retreat facilitator and organizer alongside Isaiah "Kenney" of the Holy Earth Foundation.

David's family is currently facing financial hardship. This site exists to give him a home online — a place to be found, to share his art and his teaching, and, when the world is ready to meet him there, to be supported.

**Founder & Subject:** Maestro David Amaringo
**Sponsor:** Isaiah "Kenney" (Holy Earth Foundation)
**Developer / builder:** Christopher Wilson (`drasticstatic`)
**AI agent:** Alfred (Claude Code CLI)

---

<a id="the-goal"></a>
## 🎯 The Goal

Give David a simple, dignified home online while Kenney gathers the fuller picture of his story, services, and needs — a **dev portal / concept prototype** today, not a finished commercial site. Every asset currently on the site is a placeholder, standing in until real photography, artwork scans, and copy arrive.

- **Showcase, not storefront** — his visionary art and teaching lineage, presented with care, nothing offered for direct sale yet (see [Architecture](#architecture) for the GitHub Pages compliance stance)
- **Neo-Amazónico identity** — a deep jungle-canopy palette with a rainbow flourish reserved for art-showcase moments, echoing the visionary-art tradition's own gold linework
- **Donation-ready, web3-aware** — Ayahuasca work carries payment-processor stigma, and David lives in Peru; crypto-donation readiness is on the roadmap alongside conventional donation buttons, both fully compliant with GitHub Pages' terms
- **Sister site to `iamoneself`** — same technical family, same builder, same Chaiconi Bari community

---

<a id="architecture"></a>
## 🏗️ Architecture

- **Framework:** Next.js 15 (App Router) with `output: 'export'` — pure static, no server-side Node.js runtime at deploy time
- **Styling:** Tailwind CSS v4 + Framer Motion
- **Base Path:** env-driven via `NEXT_PUBLIC_BASE_PATH`, same mechanism as `iamoneself`
- **GitHub Pages compliance:** Pages' Acceptable Use Policy permits "donation buttons and crowdfunding links" but not sites "primarily directed at facilitating commercial transactions." This site presents David's teaching and art with **nothing for sale** — donation-only for now — which keeps it squarely compliant while still giving him something real to be found by.

```text
src/
├── app/
│   ├── page.tsx      → Home (immersive hero, placeholder art)
│   ├── services/      → What David offers, beyond artwork for sale
│   ├── about/          → His lineage, training, USKO-AYAR school
│   ├── contact/         → Placeholder — routes to iamoneself.com for now
│   ├── not-found.tsx    → 404
│   └── layout.tsx        → Root layout — inline nav/footer for now
│   └── globals.css        → Neo-Amazónico theme (jungle-canopy + rainbow accent)
└── lib/
    └── utils.ts            → cn() + getBasePath(), mirrors iamoneself
```

---

<a id="development"></a>
## 💻 Development

```bash
npm install
npm run dev
# Opens at http://localhost:3000
```

```bash
npm run build
# Produces static site in /out
```

---

<a id="collaboration"></a>
## 🤝 Collaboration

| Role | Who |
|------|-----|
| **Founder & Subject** | Maestro David Amaringo |
| **Sponsor** | Isaiah "Kenney" (Holy Earth Foundation) |
| **Developer / Builder** | Christopher Wilson |
| **Agent** | Alfred (Claude Code CLI) |

**Sister sites** in the same technical family:
- [`iamoneself`](https://github.com/drasticstatic/iamoneself) — The Holy Earth Foundation, David's home partner community
- [`findyourfeathers`](https://github.com/drasticstatic/findyourfeathers) — the more minimal-repo structural model this scaffold followed

---

<a id="license"></a>
## 📜 License

This repository is the private development source — not licensed for
reuse. Its [public preview](https://github.com/drasticstatic/david-amaringo-public-preview)
is available under the [MIT License](https://github.com/drasticstatic/david-amaringo-public-preview/blob/main/LICENSE).
