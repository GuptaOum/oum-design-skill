# Oum's Design Avengers

**A web design workflow skill for coding agents.** It turns "design me a
website" into a clear, repeatable process, calling only the tools a request
needs and falling back gracefully when one is missing.

[![Version](https://img.shields.io/github/v/release/GuptaOum/oum-design-skill?label=version)](https://github.com/GuptaOum/oum-design-skill/releases)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Cost](https://img.shields.io/badge/cost-free-success)

---

## Contents

- [Why](#why)
- [Install](#install)
- [Usage](#usage)
- [How it works](#how-it-works)
- [The team](#the-team)
- [What needs a sign-in](#what-needs-a-sign-in)
- [Built-in guides](#built-in-guides)
- [Contributing](#contributing)
- [License](#license)

---

## Why

Agents asked to "make a website" tend to produce the same generic page.
This skill gives them a design team's discipline instead:

| Problem | What the skill does |
|---|---|
| Generic, template-looking pages | Commits to **one** design direction taken from the subject |
| Too many tools, wasted effort | **Routes** each request to only the steps it needs |
| Breaks when a tool is missing | Every tool has a **written fallback** |
| Surprise logins and paid plans | Marks each tool's **needs**: none, install, connect or sign-in |
| "Looks fine in code" but not on screen | Always **verifies** in a real browser at desktop and phone sizes |

---

## Install

| Method | How |
|---|---|
| **Plugin marketplace** | `/plugin install oum-design-skill --marketplace GuptaOum/oum-design-skill` |
| **Zip upload** | Download the latest zip from [Releases](https://github.com/GuptaOum/oum-design-skill/releases) and upload it to your agent's skills |
| **Manual** | Copy `skills/oum-desing-skill/SKILL.md` into your agent's skills directory |

---

## Usage

Ask for any web design task, or start with **"assemble"**,
**"design avengers"** or **"oum design"**.

| Example request | What runs |
|---|---|
| "Design a landing page for my startup" | All 8 steps |
| "Polish my portfolio" | Research, polish, review, verify |
| "My site looks generic" | Direction, review, verify |
| "Add a particle hero" | Research, 3D guide, verify |
| "Make it feel like Apple" | Apple guide, polish, review, verify |
| "I need an animated gradient background" | Gradient guide, build, verify |

---

## How it works

```
Briefing → Research → Direction → Build → Motion → Polish → Review → Verify
   0          1           2          3       4        5        6        7
```

| Step | Goal |
|---|---|
| 0 · Briefing | Purpose, audience, main action, brand. Existing page? Ask: polish or redesign |
| 1 · Research | 3–5 real reference sites, shown as a shortlist |
| 2 · Direction | One idea for layout, type, colour and imagery |
| 3 · Build | Design tokens first, then sections, in the project's own stack |
| 4 · Motion | The right motion tool for each effect |
| 5 · Polish | Hover, focus, press states, easing, timing |
| 6 · Review | Hierarchy, spacing, contrast, copy, responsiveness |
| 7 · Verify | Screenshots on desktop and phone, console errors, stress tests |

---

## The team

Each tool is a hero with one job. They don't all fight every battle.

| Hero | Tool | Job | Step |
|---|---|---|---|
| `NF` Nick Fury | design-taste-frontend | One clear design direction | 2 |
| `DS` Doctor Strange | Awwwards | Award-winning references | 1 |
| `SW` Scarlet Witch | AnimatedWebs | Cinematic heroes and backgrounds | 1, 3 |
| `SM` Spider-Man | Scrapling | Screenshots of reference sites | 1 |
| `VI` Vision | Figma | Figma designs to code | 0 |
| `IM` Iron Man | Frontend and React skills | Builds the page | 3 |
| `FA` Falcon | shadcn/ui | Buttons, forms, menus, dialogs | 3 |
| `JA` Jarvis | Context7 | Latest library docs | 3, 4 |
| `TH` Thor | Framer Motion, GSAP, CSS | Motion | 4 |
| `WK` Wakanda | Apple design | Apple look and Liquid Glass | 2, 5 |
| `CM` Captain Marvel | Three.js, React Three Fiber, GLSL, TSL | 3D, particles, shaders | 4 |
| `RO` Rocket | Spline | 3D scenes | assets |
| `GR` Groot | Unicorn Studio | WebGL effects | assets |
| `SL` Star-Lord | LottieFiles | Animated illustrations | assets |
| `DX` Drax | Poly Haven, ambientCG | Free textures and materials | assets |
| `BW` Black Widow | emil-design-eng | Small details and micro-interactions | 5 |
| `CA` Captain America | impeccable | Honest design review | 6 |
| `HE` Hawkeye | Browser | Desktop and phone checks | 7 |
| `HU` Hulk | break-ui | Stress tests | 7 |

---

## What needs a sign-in

The skill works with **no accounts at all**. Tools marked **sign-in** add
more when connected; the agent asks before using them.

| Needs | Tools |
|---|---|
| **None** | shadcn/ui, Framer Motion, GSAP, Three.js, React Three Fiber, LottieFiles (playback), Poly Haven, ambientCG |
| **Install** (a skill) | design-taste-frontend, apple-design, emil-design-eng, impeccable, break-ui, frontend and React skills |
| **Connect** (a server, no account) | Awwwards, Scrapling, Context7, browser tool, Three.js MCP |
| **Sign-in** (your account) | AnimatedWebs (component code needs a paid plan), Figma, Spline (daily call limit), Unicorn Studio |

---

## Built-in guides

| Guide | Covers |
|---|---|
| **Motion** | When to use Framer Motion, GSAP + ScrollTrigger, Three.js or plain CSS; the universal scroll recipe |
| **3D** | How Three.js renders, vertex / fragment / compute shaders, four levels of shader code, a TSL example, GPU particles |
| **Apple** | Apple's design habits; Liquid Glass as CSS frosted glass or true refraction |
| **Assets** | Free 3D, WebGL effects, animated illustrations and CC0 textures, with licence notes |
| **Gradients** | Video export, live coded gradients, ready WebGL gradients and plain CSS |

---

## Contributing

Issues and pull requests are welcome. When adding a tool, include its job,
what it needs (none, install, connect or sign-in) and a fallback, so the
skill keeps working for everyone.

See [Releases](https://github.com/GuptaOum/oum-design-skill/releases) for the changelog.

## License

[MIT](LICENSE) © GuptaOum
