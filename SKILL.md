---
name: oum-desing-skill
description: Oum's "Design Avengers" — the end-to-end workflow for designing and building a beautiful web page or website from scratch by assembling the right design skills and MCP tools in the right order (research → direction → build → motion → polish → verify). Use this whenever the user wants to design, build, redesign or restyle a landing page, home page, event site, portfolio, marketing page, hero section or any public-facing web page, asks to make a site look premium / award-level / less generic, says "assemble", "design avengers", or "oum design", or starts a page with no design yet — even if they don't name any skill or tool.
---

# Oum's Design Avengers

A good-looking page is rarely the result of one tool. It comes from a sequence:
know what great looks like, commit to one clear direction, build it cleanly,
add motion with restraint, then look at it in a real browser and fix what's
wrong. Each "Avenger" below owns one of those stages. Your job is to be the
team lead: call each one at the right moment, carry decisions forward, and
never skip the look-and-fix loop at the end.

Load each skill **when you reach its stage**, not all up front — they are long,
and loading them early just crowds out the context you need for the page itself.

## The team

| Avenger | Tool | Stage | Power |
|---|---|---|---|
| Nick Fury | `design-taste-frontend:design-taste-frontend` (skill) | Direction | Picks the idea, type, palette, composition; bans generic "AI-made" design |
| Doctor Strange | **Awwwards MCP** (`mcp__awwwards__*`) | Research | Real award-winning references, design DNA, motion breakdowns, build scoring |
| Scarlet Witch | **AnimatedWebs MCP** + `animatedwebs:*` skills | Research / Build | Cinematic heroes, video/WebGL backgrounds, animated components |
| Spider-Man | **Scrapling MCP** | Research | Screenshots and content from any reference URL |
| Vision | **Figma MCP** | Input | Turns the user's Figma designs into code (and back) |
| Iron Man | `zizi-skills:frontend`, `react-patterns`, `vercel-react-best-practices` | Build | Clean, fast component code |
| Jarvis | **Context7 MCP** (`resolve-library-id` → `query-docs`) | Build | Current official docs for Framer Motion, GSAP, R3F, Tailwind, Next.js — see "Jarvis protocol" below |
| Professor X | Official design plugin: `design:*` skills, `artifact-design` | Review / Handoff | Official design critique, design system, accessibility, UX copy and handoff passes |
| Thor | `animate:animate`, `animation-performance:animation-performance` | Motion | Purposeful animation that stays at 60fps |
| Wakanda | `apple-design` skill | Direction / Polish | Apple-style restraint, type and spacing; Liquid Glass surfaces — see "Wakanda: Apple design and Liquid Glass" below |
| Rocket | **Spline** + official **Spline MCP** (`spline`, `https://mcp.spline.design/mcp`) | 3D assets | Build and edit 3D scenes directly, then embed with `@splinetool/react-spline` |
| Groot | **Unicorn Studio** (no MCP; user shares embed code / project ID) | WebGL effects | Ready distortion, glow, liquid and image-particle effects, embedded |
| Star-Lord | **LottieFiles** (`@lottiefiles/dotlottie-react`) | Animated art | Lightweight animated illustrations, icons and loaders |
| Gamora | **Rive** (`@rive-app/react-canvas`) | Interactive art | Animations that react to hover, clicks and state |
| Drax | **Poly Haven**, **ambientCG** (CC0) | Textures | Free PBR materials, HDRI lighting and 3D models for Three.js / R3F |
| Captain Marvel | **React Three Fiber + Three.js + GLSL shaders**, Three.js MCP (`learn_threejs`, `show_threejs_scene`), AnimatedWebs WebGL gradients | 3D / WebGL | Particles, 3D scenes, shader backgrounds, GPU physics — see "Captain Marvel's lab" below |
| Black Widow | `emil-design-eng:emil-design-eng` | Polish | Easing, timing, hover/press states, invisible details |
| Captain America | `impeccable:impeccable` | Review | Hierarchy, layout, spacing, color, copy, accessibility |
| Hawkeye | Built-in browser pane / browser extension | Verify | Screenshots at desktop + mobile, dark mode, console errors |
| Hulk | `break-ui:break-ui` | Verify | Smashes the page with long text, empty states, odd viewports |

Reserves (call when the page needs them): `theme-factory`
(fast theme), `mobile-native` (phone feel), `design-skills:ux-writing`
(headlines, buttons), `design-skills:accessibility-audit`,
`web-design-guidelines:web-design-guidelines`, Canva MCP (posters/social graphics).

**Call the team selectively.** Pick only the members the request needs (see
"Scaling the mission"); never load every skill or hit every MCP by default.
Name the members you are calling and why in one line before starting.

## S.H.I.E.L.D. archive: every design skill, by job

The full index of design skills installed for this user. Load one only when
its job comes up; use the exact name shown.

| Job | Skills |
|---|---|
| Direction, taste, anti-generic | `design-taste-frontend:design-taste-frontend`, `design-skills:design-elevation`, `zizi-skills:design-guide`, `apple-design` |
| Modern web platform and standards | `modern-web-guidance:modern-web-guidance` (current CSS/HTML/browser APIs), `web-design-guidelines:web-design-guidelines` |
| Building pages and components | `zizi-skills:frontend`, `react-patterns`, `vercel-react-best-practices`, `nextjs-turbopack`, `zizi-skills:tabler-ui` (dashboards) |
| Motion | `animate:animate`, `animation-vocabulary:animation-vocabulary` (name the effect you want), `animation-performance:animation-performance`, `emil-design-eng:emil-design-eng` |
| Interaction and UX | `design-skills:interaction-design`, `design-skills:ux-strategy`, `design-skills:journey-mapping`, `zizi-skills:information-architecture` |
| Critique and review | `impeccable:impeccable`, `design:design-critique`, `design-skills:design-critique` |
| Design systems and tokens | `design:design-system`, `design-skills:design-systems`, `design-skills:design-ops`, `animatedwebs:style`, `theme-factory` |
| Copy and words on the page | `design:ux-copy`, `design-skills:ux-writing`, `zizi-skills:plain-language` |
| Accessibility | `design:accessibility-review`, `design-skills:accessibility-audit`, `chrome-devtools-mcp:a11y-debugging` |
| Research | `design:user-research`, `design:research-synthesis`, `design-skills:ux-research` |
| Handoff from Figma | `design:design-handoff` (+ Figma MCP) |
| 3D, WebGL effects and animated art (tools, not skills — see the Guardians' asset bay) | **Spline** (Spline MCP `spline`), **Unicorn Studio** (embed), **LottieFiles** (`@lottiefiles/dotlottie-react`), **Rive** (`@rive-app/react-canvas`), **Poly Haven / ambientCG** (textures), React Three Fiber + GLSL + Three.js MCP |
| Ready-made animated pieces | `animatedwebs:hero`, `animatedwebs:background`, `animatedwebs:gradient`, `animatedwebs:component`, `animatedwebs:site`, `animatedwebs:browse` |
| Graphics and art | `zizi-skills:design-assets`, `canvas-design` (posters, static art), `algorithmic-art` (generative p5.js) |
| Phone feel | `mobile-native` |
| Speed and stress tests | `chrome-devtools-mcp:debug-optimize-lcp`, `break-ui:break-ui` |
| Shareable artifact pages | `artifact-design` |

## Thor's armoury: pick the right motion tool

Motion libraries animate what you've built; they are not design frameworks
(not like Material UI). Choose **one** primary tool per effect, by what the
effect is, and match the project's stack:

| The effect is… | Use | Why |
|---|---|---|
| UI motion in a React app: hover/press, fade-up on enter, layout and tab transitions, page transitions | **Framer Motion** (`motion`): `motion.div`, `whileInView`, `layoutId`, `AnimatePresence` | Lives in the JSX, React-native, light |
| Scroll-driven scenes in React: pinned stage, values tied to scroll | **Framer Motion**: sticky CSS stage + scroll progress → `useSpring` → `useTransform` → `motion.*` `style` | Updates the element every frame without React re-renders |
| Long, cinematic, multi-step timelines; award-style sequences; non-React or mixed stacks; SVG/morph/text splitting | **GSAP** + **ScrollTrigger** (in React via `@gsap/react` `useGSAP` with refs) | Most powerful timeline and scroll-pinning engine |
| Thousands to millions of particles, 3D, shaders, real physics, GPU simulation | **React Three Fiber / Three.js + GLSL** | GSAP/Framer can't draw on a GPU canvas or run per-particle physics; they may only tween shader uniforms or camera on top |
| Simple hover/focus states and one-shot reveals | **Plain CSS** transitions/keyframes + `IntersectionObserver` | No library needed |

Rules:
- Don't add GSAP to a project already using Framer Motion (or the reverse)
  unless one effect genuinely needs it; say why if you do.
- The scroll-animation workflow for any library: **sticky stage → scroll
  progress 0–1 → map progress to values → apply as styles.**
- Always respect `prefers-reduced-motion` with a static fallback, and pause
  render loops / videos when offscreen (`IntersectionObserver`).
- Comparing libraries for the user: build the same small effect in each,
  using Context7 for each library's current API.

## Wakanda: Apple design and Liquid Glass

Load `apple-design` when the user asks for an Apple-like look (apple.com
product pages, macOS/iOS feel, "premium and minimal") or for Liquid Glass.
Apple's habits: one idea per screen, big confident type, generous space,
real product imagery, motion that explains rather than decorates.

Liquid Glass on the web comes in two levels; pick the cheapest that reads right:
1. **Frosted glass (CSS, default):** semi-transparent fill,
   `backdrop-filter: blur(20–30px) saturate(150%)`, a 1px light edge
   (`inset 0 0 0 1px rgba(255,255,255,.1)`), a brighter top highlight and a
   soft shadow. Works everywhere, cheap. Use for navbars, cards, menus.
2. **True refraction (shader):** the glass bends what's behind it like a
   lens. Needs an SVG displacement filter (`feDisplacementMap`, Chromium-only)
   or a GLSL refraction shader in React Three Fiber (Captain Marvel's lab).
   Use only for one hero moment, never for every surface.
Always keep text on glass readable (check contrast) and give a solid fallback
when `backdrop-filter` or WebGL is unavailable.

## The Guardians' asset bay: plug-and-play art, 3D and textures

Rocket (Spline), Groot (Unicorn Studio), Star-Lord (LottieFiles), Gamora
(Rive) and Drax (Poly Haven / ambientCG). Details:

When the page needs animated art, 3D or textures that don't exist yet, use
free sources before drawing anything by hand. Check each asset's licence
before shipping and credit it where the licence asks.

| Need | Source (free) | How it plugs in |
|---|---|---|
| Animated illustrations, icons, loaders | **LottieFiles** (free animations, JSON / .lottie) | `@lottiefiles/dotlottie-react` or `lottie-web` |
| Interactive animations that react to hover/clicks | **Rive** community files (free tier) | `@rive-app/react-canvas` |
| 3D scenes you can embed without coding 3D | **Spline** (free tier) — official **Spline MCP** (`spline`, `https://mcp.spline.design/mcp`) lets the agent build and edit scenes directly; calls count against a daily allowance | `@splinetool/react-spline` or iframe embed |
| Ready WebGL effects (distortion, glow, particles on images) | **Unicorn Studio** (free tier; no MCP — the user designs the effect in its editor and shares the project ID / embed code) | Its embed script, lazy-loaded |
| Animated WebGL gradient backgrounds | **AnimatedWebs** Gradient Studio | `animatedwebs:gradient` skill |
| Textures, PBR materials (metal, concrete, fabric), HDRI lighting, 3D models | **Poly Haven** and **ambientCG** (CC0, fully free) | Three.js / R3F materials and `useTexture` |
| Real photos, maps, engravings, footage of the subject's world | Open collections via design-taste's `assets.mjs` (Openverse, Wikimedia, museums) | `public/` images, credited |
| Shader ideas | **Shadertoy** | Study only: most shaders there are non-commercial licence, so rewrite, don't copy |

Rules: prefer the project's own media first; keep files light (compress
video, cap Lottie size, lazy-load embeds); pause animations offscreen; and
never present a generic asset as the client's own product.

## Captain Marvel's lab: WebGL, GLSL and React Three Fiber

Reach for this only when the effect really needs the GPU: particle images,
3D objects or scenes, shader-driven backgrounds, distortion, or physics on
thousands of points. A gradient or shader *background* that already exists is
cheaper: try AnimatedWebs' WebGL gradients (`animatedwebs:gradient`) first.

The stack (all free):
- **Three.js**: the WebGL engine (scenes, cameras, materials, geometry).
- **React Three Fiber (R3F)**: Three.js as React components: `<Canvas>`,
  `<mesh>`, `useFrame` for the per-frame loop, `useThree` for the renderer.
- **@react-three/drei**: ready helpers (orbit controls, text, environment,
  loaders); check it before hand-writing a helper.
- **GLSL shaders**: small GPU programs. *Vertex* shaders place each point,
  *fragment* shaders colour each pixel. Write them in `.glsl` files imported
  as strings (`import frag from "./x.frag.glsl?raw"`) and pass data in with
  uniforms (every frame, same for all), attributes (once per point) and
  textures.
- **GPGPU** (simulation on the GPU): store each particle's position and
  velocity in float textures and update them with shaders every frame
  (`GPUComputationRenderer` handles the ping-pong). This is how an image
  becomes up to ~1M particles that react to the mouse; plain JS on a 2D
  canvas tops out near ~20k at 60 fps.

How to use it:
- Prototype or explain a scene with the Three.js MCP (`learn_threejs`,
  `show_threejs_scene`), then build it in the project with R3F.
- Check current APIs via the Jarvis protocol: `@react-three/fiber`,
  `@react-three/drei`, `three` (versions change often).
- GSAP or Framer Motion may sit *on top*: tween a shader uniform, the camera,
  or tie a uniform to scroll progress. They never replace the shaders.

Performance and safety rules (always):
- Pause the render loop when the canvas is offscreen (`IntersectionObserver`
  → `frameloop="never"`/`"demand"`), and when the tab is hidden.
- Cap pixel ratio (`dpr={[1, 2]}`), keep particle counts lower on phones, and
  dispose geometries, materials, textures and render targets on unmount.
- Provide a static image fallback for `prefers-reduced-motion` and for
  devices without WebGL or float-texture support (try `HalfFloatType`).
- Uniform/attribute names must match exactly between JS and GLSL; a typo
  silently gives 0, so check names first when nothing moves.

## Jarvis protocol: Context7 before writing library code

Library APIs change (Framer Motion is now published as `motion`; GSAP
plugins and React Three Fiber versions move). Before writing non-trivial code
for a library, fetch its current docs instead of relying on memory:
1. `resolve-library-id` with the library name (e.g. "framer motion", "gsap",
   "react three fiber", "tailwindcss", "next.js").
2. `query-docs` with that id and the specific question ("useScroll with
   sticky section", "ScrollTrigger pin with React useGSAP").
Use the version in the project's `package.json` when the docs differ.

## Professor X: official design plugin tools

The official design plugin skills, for a second, principled opinion:
- `design:design-critique` — structured feedback on hierarchy, usability,
  consistency (run alongside `impeccable` in stage 6).
- `design:design-system` — audit tokens/components for drift and hardcoded values.
- `design:accessibility-review` — WCAG checks before shipping.
- `design:ux-copy` — headlines, buttons, empty and error states.
- `design:design-handoff` — specs for developers when the design came from Figma.
- `artifact-design` — the design contract when the deliverable is a shareable
  artifact page rather than the user's codebase.

If a tool isn't available in the session (MCP not connected, skill missing),
say so in one line and continue with the rest of the team — the workflow still
works without any single member.

## The mission (run in this order)

### 0. Briefing — understand the page
Before designing anything, get clear on: what the page is for, who it's for,
the one action a visitor should take, the content that must appear, and any
existing brand (logo, colors, fonts) or Figma file. Read the project to learn
the stack (React? Tailwind? Next?) so the build matches it.

Ask only what you can't infer. If the user has a Figma link, call in Vision
first and treat that design as the direction (skip most of stage 2).

**If the page already exists, ask before anything else: polish or redesign?**
Open it in the browser, look at it and skim its code, then ask the user with
the structured question tool (or in one line if there is none). Offer:
- **Critique + polish** — keep the design and structure; fix what the checks
  find. Runs stages 1 (light), 5, 6, 7.
- **Critique only** — a written list of findings, no code changes.
- **Full redesign, kept separate** — a new design as a separate page or on a
  new git branch, so the current one stays untouched for comparison.

Describe what you saw (its look, its main sections, how big it is) so the
user can decide without opening it themselves. Recommend polish when the page
already has a clear direction, and redesign only when it looks generic or
broken. Why ask: an existing page is someone's recent work, and a redesign
throws it away. A "redesign" request about a well-built page usually means
"make it better", which polish does without the loss. Skip the question only
when the user has already said which they want.

### 1. Research — Doctor Strange, Spider-Man, Scarlet Witch
Find 3–5 real references close to the page's purpose and mood.
- `mcp__awwwards__search_sites` (filters: tags, colors, technology, award) →
  `get_site_details` / `compare_sites` for palette, type, stack, elements.
- `mcp__awwwards__create_design_brief` turns 2–5 chosen slugs plus the
  project goal into a cited brief — a strong handoff into stage 2.
- AnimatedWebs `search_catalog` for heroes/backgrounds/components worth reusing.
- Scrapling `screenshot` / `get` for any non-Awwwards reference the user names.

Show the user the shortlist (name, why it fits) and let them react — taste is
theirs to decide. References are for learning patterns, never for copying a
site wholesale; Awwwards data is for personal, non-commercial inspiration.

### 2. Direction — Nick Fury
Load `design-taste-frontend:design-taste-frontend` and follow it to commit to **one**
direction: the idea, composition, type pairing, palette, imagery, and a
section-by-section blueprint. Feed it what stage 1 learned. Write the decision
down briefly (in the reply or a short DESIGN.md if the project keeps one) so
later stages don't drift.

Why one direction: mixing three references produces mush. A single, confident
idea is what makes a page look designed.

### 3. Build — Iron Man + Jarvis
Build in the project's own stack and conventions. Use Context7 for library APIs
instead of guessing. Set design tokens (color, type scale, spacing, radius) as
variables first, then build sections top to bottom. Use AnimatedWebs components
or backgrounds where they fit the direction rather than hand-rolling effects.

### 4. Motion — Thor (+ Doctor Strange for reference motion)
Load `animate:animate`. Decide per element whether it should move at
all, then purpose, property, curve, duration. Pick the library from "Thor's
armoury" above and check its API through the Jarvis protocol (Context7). If a reference site's motion is
the target, study it with `mcp__awwwards__analyze_scroll_map`,
`analyze_hover_census` or `get_motion_dna` (these need Playwright — installed
globally on this machine), and optionally `build_gsap_stub`.
If anything stutters, load `animation-performance:animation-performance`.
Always respect `prefers-reduced-motion`.

### 5. Polish — Black Widow
Load `emil-design-eng:emil-design-eng` and pass over every interactive
element: hover/focus/active states, transition timing and easing, entrance
choreography, tap feedback on mobile.

### 6. Review — Captain America
Load `impeccable:impeccable` and critique the page honestly: hierarchy,
alignment, spacing rhythm, color contrast, copy, responsive behavior. Fix what
it finds before moving on.

### 7. Verify — Hawkeye + Hulk (do not skip)
Code that compiles is not a page that looks right. Start the dev server with
the browser pane (`preview_start`), then:
- screenshot at desktop and mobile (`resize_window` preset `mobile`), and dark
  mode if the site supports it;
- check console errors;
- load `break-ui:break-ui` for long text, empty states, narrow widths;
- optionally `mcp__awwwards__verify_build` against the chosen reference, and
  `analyze_accessibility` / `audit_url` for evidence on contrast and perf.

Fix, re-screenshot, repeat until it holds up. Then show the user the final
screenshots.

## Scaling the mission
Not every request needs the full team.
- **Whole page or site from scratch** → all stages.
- **Existing page** → ask polish or redesign first (stage 0). Polish runs
  1 (light), 5, 6, 7; redesign runs all stages, kept separate from the old page.
- **Just a hero / one section** → 1 (AnimatedWebs first), 2 (light), 3, 4, 7.
- **"It looks generic / AI-made"** → 2 and 6 are the heart; then 7.
- **"Animations feel off"** → 4, 5, 7.
- **3D, particles, shaders or a WebGL background** → 1 (AnimatedWebs and
  Awwwards for references), Captain Marvel's lab, 4, 7.
- **"Make it look like Apple" / Liquid Glass** → Wakanda (`apple-design`),
  then 2, 5, 6, 7.
- **"I need art / textures / animated illustrations"** → the Guardians'
  asset bay (Spline for 3D, Unicorn Studio for WebGL effects, LottieFiles or
  Rive for animated art, Poly Haven / ambientCG for textures), then 3 and 7.

## Reporting back
End with: what direction was chosen and why (one or two lines), which
references inspired it, screenshots (desktop + mobile), and anything not done
or not verified.
