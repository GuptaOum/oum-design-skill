# 🛡️ Oum's Design Avengers

**An end-to-end web design workflow skill for coding agents.**
It turns "design me a website" into a disciplined mission, assembling the right
design tools in the right order, and only the ones the job needs.

| | |
|---|---|
| **What it is** | A single agent skill (`SKILL.md`) packaged as a plugin |
| **What it builds** | Landing pages, home pages, portfolios, event sites, product pages, hero sections |
| **Version** | 1.2.0 |
| **Cost** | Free. Every tool it relies on has a free route |
| **License** | MIT |

---

## Install

| Method | Steps |
|---|---|
| **Plugin marketplace** (recommended) | `/plugin install oum-design-skill --marketplace GuptaOum/oum-design-skill` |
| **Marketplace, two-step** | `/plugin marketplace add GuptaOum/oum-design-skill` then `/plugin install oum-design-skill@oum-design` |
| **Zip upload** | Download the zip from [Releases](https://github.com/GuptaOum/oum-design-skill/releases) and upload it to your agent's skills |
| **Manual** | Copy `skills/oum-desing-skill/SKILL.md` into a folder named `oum-desing-skill` in your agent's skills directory |

### Trigger it

Ask to design, build, redesign or restyle any public web page, or say any of:

| Phrase | Example |
|---|---|
| `assemble` | "Assemble and redesign my portfolio" |
| `design avengers` | "Design avengers, build a launch page" |
| `oum design` | "Oum design this hero section" |
| "make it premium / award-level / less generic" | "This page looks AI-made, fix it" |

---

## The mission: 7 stages

| # | Stage | Who | What happens |
|---|---|---|---|
| 0 | **Briefing** | — | Purpose, audience, one main action, brand. For an existing page: asks *polish or redesign?* first |
| 1 | **Research** | Doctor Strange, Spider-Man, Scarlet Witch | 3–5 real award-winning references, shown to you as a shortlist |
| 2 | **Direction** | Nick Fury, Wakanda | Commits to **one** idea: type, palette, composition, imagery |
| 3 | **Build** | Iron Man, Jarvis | Design tokens first, then sections top to bottom, in your stack |
| 4 | **Motion** | Thor, Captain Marvel | Picks the right motion tool, checks its current docs |
| 5 | **Polish** | Black Widow | Hover, focus, press states, easing, timing |
| 6 | **Review** | Captain America, Professor X | Honest critique of hierarchy, spacing, colour, copy, accessibility |
| 7 | **Verify** | Hawkeye, Hulk | Desktop + phone screenshots, console errors, stress tests, repeat until it holds |

### Scaling: not every job needs every stage

| Request | Stages run |
|---|---|
| Whole page or site from scratch | All |
| Polish an existing page | 1 (light), 5, 6, 7 |
| Just a hero or one section | 1, 2 (light), 3, 4, 7 |
| "It looks generic / AI-made" | 2 and 6, then 7 |
| "Animations feel off" | 4, 5, 7 |
| 3D, particles, shaders, WebGL background | 1, Captain Marvel's lab, 4, 7 |
| "Make it look like Apple" / Liquid Glass | Wakanda, 2, 5, 6, 7 |
| "I need art, textures, animated illustrations" | The Guardians' asset bay, 3, 7 |

---

## The team: 20 members

### Core squad

| Avenger | Tool | Stage | Power |
|---|---|---|---|
| **Nick Fury** | `design-taste-frontend` | Direction | One committed idea; bans generic, template-looking design |
| **Doctor Strange** | Awwwards MCP | Research | Award-winning references, design DNA, motion breakdowns |
| **Scarlet Witch** | AnimatedWebs | Research / Build | Cinematic heroes, video and WebGL backgrounds, animated components |
| **Spider-Man** | Scrapling | Research | Screenshots and content from any reference site |
| **Vision** | Figma MCP | Input | Figma designs to code and back |
| **Iron Man** | Frontend and React skills | Build | Clean, fast component code |
| **Jarvis** | Context7 | Build | Current official docs before writing library code |
| **Professor X** | Official design plugin skills | Review / Handoff | Critique, design system, accessibility, UX copy, handoff |
| **Thor** | `animate`, `animation-performance` | Motion | Purposeful motion that stays at 60 fps |
| **Wakanda** | `apple-design` | Direction / Polish | Apple-style restraint and Liquid Glass |
| **Captain Marvel** | React Three Fiber, Three.js, GLSL, TSL | 3D / WebGL | Particles, 3D scenes, shader backgrounds, GPU physics |
| **Black Widow** | `emil-design-eng` | Polish | Easing, timing, micro-interactions |
| **Captain America** | `impeccable` | Review | Hierarchy, layout, spacing, colour, copy |
| **Hawkeye** | Browser | Verify | Screenshots at desktop and phone sizes, console errors |
| **Hulk** | `break-ui` | Verify | Long text, empty states, odd viewports |

### Guardians: free asset tools

| Guardian | Tool | Gives you | Plugs in with |
|---|---|---|---|
| **Rocket** | Spline (official MCP) | 3D scenes built and edited by the agent | `@splinetool/react-spline` |
| **Groot** | Unicorn Studio | Distortion, glow, liquid and image-particle effects | Embed script |
| **Star-Lord** | LottieFiles | Animated illustrations, icons, loaders | `@lottiefiles/dotlottie-react` |
| **Gamora** | Rive | Animations that react to hover, clicks and state | `@rive-app/react-canvas` |
| **Drax** | Poly Haven, ambientCG (CC0) | PBR materials, HDRI lighting, 3D models | Three.js / R3F textures |

---

## Built-in guides

### Thor's armoury: which motion tool?

| The effect is… | Use |
|---|---|
| UI motion in React: hover, fade-up, tab and page transitions | **Framer Motion** |
| Scroll-driven scenes in React | **Framer Motion**: sticky stage → scroll progress → `useTransform` |
| Long cinematic timelines, non-React sites, SVG morphs, text splitting | **GSAP + ScrollTrigger** |
| Thousands to millions of particles, 3D, shaders, physics | **React Three Fiber + Three.js + GLSL / TSL** |
| Simple hovers and one-shot reveals | **Plain CSS** |

**Universal scroll recipe:** sticky stage → progress 0–1 → map to values → apply as styles.

### Animated gradients

| You want | Tool | Output |
|---|---|---|
| A gradient **video** | Gradient maker by Juan Garcia | MP4 loops, stills up to 4K |
| A **live, coded** flowing gradient | ShaderGradient or Paper Shaders | React component |
| A ready WebGL gradient | AnimatedWebs Gradient Studio | Drop-in hero background |
| A slow colour drift | Plain CSS | No library |

### Captain Marvel's lab: shaders in four levels

| Level | How | When |
|---|---|---|
| 1 | Built-in materials | No shader code needed; use first |
| 2 | `onBeforeCompile` | Small twist on a built-in material |
| 3 | `ShaderMaterial` / `RawShaderMaterial` | Fully custom GLSL |
| 4 | **TSL** (Three.js Shading Language) | Shaders written in JavaScript, compiled to WGSL (WebGPU) or GLSL (WebGL) |

| Shader type | Runs once per | Job |
|---|---|---|
| Vertex | Corner (vertex) | Where things go |
| Fragment | Pixel | What colour each pixel is |
| Compute | Data item | Number-crunching (real on WebGPU, emulated with textures on WebGL) |

### Wakanda: Liquid Glass in two levels

| Level | Technique | Use for |
|---|---|---|
| Frosted glass | CSS `backdrop-filter`, translucent fill, light edge | Navbars, cards, menus |
| True refraction | SVG displacement or a GLSL refraction shader | One hero moment only |

### Jarvis protocol

| Step | Action |
|---|---|
| 1 | Resolve the library in Context7 (Framer Motion, GSAP, R3F, Tailwind, Next.js…) |
| 2 | Query the exact question ("ScrollTrigger pin with useGSAP") |
| 3 | Match the version in the project's `package.json` |

---

## S.H.I.E.L.D. archive

`SKILL.md` also carries a full index of about 45 design skills grouped by job:
direction, web standards, building, motion, UX, critique, design systems,
copy, accessibility, research, handoff, animated components, art, phone feel,
performance and shareable pages. It uses exact names so the right one loads.

---

## Rules it always follows

| Rule | Why |
|---|---|
| Calls only the tools the job needs, and names them first | Fast, focused, no wasted context |
| One design direction, never a mix | Mixing references produces mush |
| Respects `prefers-reduced-motion` | Accessibility |
| Pauses video, WebGL and animation off screen | Battery and smooth scrolling |
| Checks every asset's licence | Safe to ship |
| Verifies in a real browser before calling it done | Code that compiles isn't a page that looks right |
| Missing tool? Says so and carries on | Works with any subset of tools |

---

## License

MIT © GuptaOum
