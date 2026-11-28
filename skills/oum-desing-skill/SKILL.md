---
name: oum-desing-skill
description: Oum's "Design Avengers" — an end-to-end workflow for designing and building a polished web page (landing page, home page, portfolio, event or product page, hero section) in the right order — research, direction, build, motion, polish, review, verify — calling only the tools the request needs, with a fallback for every tool. Use it whenever the user wants to design, build, redesign or restyle a public web page, asks to make one look premium, award-level or less generic, asks for motion, 3D, WebGL, gradients or an Apple-style look, or says "assemble", "design avengers" or "oum design".
---

# Oum's Design Avengers

A good page comes from a sequence: know what great looks like, commit to one
direction, build it cleanly, add motion with restraint, then look at it in a
real browser and fix what's wrong. Each hero below owns one job. You are the
team leader: call only the heroes the request needs, in order, and never skip
the final look-and-fix.

## How to use this skill

1. **Route the request.** Find the closest row in the routing table and run
   only those steps.
2. **For each step, check the toolbox.** If the tool is available, use it.
   If it isn't, or it needs a sign-in the user hasn't done, use the fallback.
   Never stop because a tool is missing.
3. **Say your plan in one line** before starting: which steps and tools, and
   any tool that needs the user to connect or sign in first.
   **Ask for better tools when they'd help.** If the request would clearly
   gain from a `connect` or `sign-in` tool that isn't set up (for example a
   Figma file, a Spline 3D scene, AnimatedWebs heroes, live reference
   screenshots), tell the user once, before building, in this form:
   *"This would be better with **<tool>**: <what it adds>. It needs
   <connect / sign-in / paid plan>. Set it up, or should I continue with
   <fallback>?"* Mention only the tools that matter for this request (at
   most three), never block on the answer if the user says continue, and
   don't ask again for the same tool in the same task.
4. **Finish with step 7 (Verify).** Code that compiles is not a page that
   looks right.

## Routing: what to run for each request

| The user asks for… | Run |
|---|---|
| A new page or site from scratch | 0 → 7, all steps |
| An existing page: "polish", "improve", "fix the design" | 0 (ask polish or redesign), 1 (light), 5, 6, 7 |
| "It looks generic / AI-made / cheap" | 2, 6, 7 |
| A single hero or section | 1, 2 (light), 3, 4, 7 |
| "Animations feel off" or new motion | 4, 5, 7 |
| 3D, particles, shaders, WebGL background | 1, 4 with the 3D guide, 7 |
| "Make it look like Apple" / Liquid Glass | 2 with the Apple guide, 5, 6, 7 |
| Art, 3D models, textures, animated illustrations | Asset guide, then 3, 7 |
| A custom animated gradient | Gradient guide, then 3, 7 |

## The steps

**0. Briefing.** Learn the page's purpose, audience, the one action a
visitor should take, the content, and any brand (logo, colours, fonts) or
Figma file. Read the project to learn its stack. Ask only what you can't
infer. If the page already exists, look at it first, then ask: **polish**
(keep the design, fix issues), **critique only**, or **full redesign kept
separate** (new branch or page). Recommend polish unless it looks generic
or broken.

**1. Research.** Find 3–5 real references close to the page's purpose and
mood, and show the user a short list with one line on why each fits. Learn
patterns; never copy a site.

**2. Direction.** Commit to **one** idea: composition, type pairing, palette,
imagery and a section-by-section plan, taken from the subject itself rather
than category defaults. Write it down briefly so later steps don't drift.
Mixing three references produces mush.

**3. Build.** Use the project's own stack. Set design tokens first (colour,
type scale, spacing, radius) as variables, then build sections top to
bottom. Use the general component library for everyday UI. Check library
APIs in current docs before writing non-trivial code.

**4. Motion.** For each element decide whether it should move at all, then
its purpose, property, curve and duration. Pick the tool from the motion
guide. Respect `prefers-reduced-motion`.

**5. Polish.** Every interactive element gets hover, focus-visible, active
and disabled states; consistent easing and timing; tap feedback on phones.

**6. Review.** Critique honestly: hierarchy, alignment, spacing rhythm,
colour contrast (body text ≥ 4.5:1), copy, responsive layout. Fix what you
find before moving on.

**7. Verify.** Run the page in a real browser. Screenshot at desktop and
phone widths (and dark mode if supported), check the console for errors,
stress it with long text, empty states and narrow screens. Fix and repeat
until it holds up, then show the user the screenshots.

## Toolbox

**Needs:** `none` works immediately · `install` add a package or skill ·
`connect` add an MCP server, no account · `sign-in` the user must log in
to an account before it works. Tell the user before using a `sign-in` tool.

| Hero | Step | Tool | Job | Needs | If missing |
|---|---|---|---|---|---|
| Doctor Strange | 1 | Awwwards MCP | Award-winning references, design DNA, motion analysis | connect | Search the web for award-winning sites in the same category |
| Spider-Man | 1 | Scrapling MCP | Screenshots and content of any reference URL | connect | Open the URL in the browser tool and screenshot it |
| Scarlet Witch | 1, 3 | AnimatedWebs MCP | Cinematic heroes, video and WebGL backgrounds, animated components | **sign-in** (component code needs a paid plan) | Build the hero with the motion or 3D guide |
| Vision | 0 | Figma MCP | Turns the user's Figma design into code | **sign-in** | Ask for screenshots of the design |
| Nick Fury | 2 | `design-taste-frontend` skill | Commits to one non-generic direction | install | Follow step 2 above |
| Wakanda | 2, 5 | `apple-design` skill | Apple-style restraint and Liquid Glass | install | Follow the Apple guide below |
| Iron Man | 3 | Frontend and React skills | Clean, fast component code | install | Follow the project's own conventions |
| Falcon | 3 | **shadcn/ui** | The one general component library: buttons, forms, dialogs, menus, tabs, cards | none (npm) | Build simple accessible components by hand |
| Jarvis | 3, 4 | Context7 MCP | Current official docs for any library | connect | Read the library's official docs site |
| Thor | 4 | `animate` skill + Framer Motion / GSAP / CSS | Purposeful motion at 60 fps | install / none | Use the motion guide below |
| Captain Marvel | 4 | Three.js, React Three Fiber, GLSL, TSL; Three.js MCP | 3D, particles, shaders, GPU physics | none (npm); MCP: connect | Use the 3D guide below |
| Rocket | assets | Spline + Spline MCP | Build and edit 3D scenes, embed them | **sign-in** (Spline account; daily call allowance) | Embed a public Spline scene URL, or use Three.js |
| Groot | assets | Unicorn Studio | Ready WebGL effects: distortion, glow, liquid | **sign-in** (user designs it and shares the embed code) | Use the 3D guide or a gradient tool |
| Star-Lord | assets | LottieFiles | Animated illustrations, icons, loaders | none to play; free account to download many files | Use CSS or SVG animation |
| Drax | assets | Poly Haven, ambientCG | Free CC0 textures, materials, HDRIs, 3D models | none | — |
| Black Widow | 5 | `emil-design-eng` skill | Easing, timing, micro-interactions | install | Follow step 5 above |
| Captain America | 6 | `impeccable` skill | Design critique and fixes | install | Follow step 6 above |
| Hawkeye | 7 | Browser tool (built-in pane, browser extension or Playwright) | Screenshots, console errors, responsive checks | connect | Ask the user to check and share screenshots |
| Hulk | 7 | `break-ui` skill | Stress-tests long text, empty states, odd sizes | install | Follow step 7 above |

## Motion guide: pick one tool per effect

| The effect is… | Use |
|---|---|
| UI motion in React: hover, fade-up on enter, tab and page transitions | **Framer Motion** (`motion.div`, `whileInView`, `layoutId`, `AnimatePresence`) |
| Scroll-driven scenes in React (pinned stage, values tied to scroll) | **Framer Motion**: sticky stage → scroll progress → `useSpring` → `useTransform` → `style` |
| Long cinematic timelines, non-React sites, SVG morphs, text splitting | **GSAP + ScrollTrigger** (in React via `@gsap/react` `useGSAP` with refs) |
| Thousands of particles, 3D, shaders, physics | **Three.js / React Three Fiber** (see the 3D guide) |
| Simple hovers and one-shot reveals | **Plain CSS** transitions + `IntersectionObserver` |

Rules: don't add GSAP to a Framer Motion project (or the reverse) without a
reason. Any scroll animation follows **sticky stage → progress 0–1 → map to
values → apply as styles**. Pause animation and video when off screen.

## 3D guide: Three.js, React Three Fiber, shaders

Use it only when the effect needs the GPU. For a ready-made shader background,
try a gradient tool first.

**How rendering works.** JavaScript describes the scene; Three.js turns it
into GPU commands and shader code; the browser compiles the shaders once and
reuses them every frame. `WebGLRenderer` is the default and works everywhere;
`WebGPURenderer` is newer and falls back to WebGL.

**Shader types:** *vertex* places each corner, the GPU fills in the pixels
inside each triangle, *fragment* colours each pixel, *compute* crunches data
(real on WebGPU, emulated on WebGL by rendering into textures).

**Where shader code comes from, cheapest first:**
1. Built-in materials (`MeshStandardMaterial`, `PointsMaterial`…): no shader code.
2. `onBeforeCompile`: patch a built-in material.
3. `ShaderMaterial` / `RawShaderMaterial`: your own GLSL in `.glsl` files (`?raw` imports).
4. **TSL**: shaders written in JavaScript, compiled to WGSL or GLSL.

```js
import * as THREE from "three/webgpu";
import { Fn, uv, time, sin, mix, color } from "three/tsl";

const material = new THREE.MeshBasicNodeMaterial();
material.colorNode = Fn(() => {
  const t = sin(time.add(uv().x.mul(3))).mul(0.5).add(0.5); // 0..1 wave over time
  return mix(color("#1d1e22"), color("#a4a6ab"), t);        // graphite → silver
})();
const renderer = new THREE.WebGPURenderer(); // falls back to WebGL
```

TSL and WebGPU APIs change often: check current docs before writing them.

**Particles at scale:** store each particle's position and velocity in float
textures and update them with shaders every frame (ping-pong), or use TSL
compute on WebGPU. Plain JavaScript on a 2D canvas tops out near 20,000
particles at 60 fps; the GPU handles about a million.

**Always:** pause the render loop off screen and when the tab is hidden; cap
pixel ratio (`dpr={[1, 2]}`); use fewer particles on phones; dispose GPU
resources on unmount; show a still image for reduced motion or no WebGL;
match uniform and attribute names exactly between JS and GLSL (a typo
silently gives 0).

## Apple guide: Apple look and Liquid Glass

Apple's habits: one idea per screen, big confident type, generous space, real
product imagery, motion that explains rather than decorates.

| Liquid Glass level | How | Use for |
|---|---|---|
| Frosted glass (default) | Translucent fill, `backdrop-filter: blur(20–30px) saturate(150%)`, 1px light edge, brighter top highlight, soft shadow | Navbars, cards, menus |
| True refraction | SVG `feDisplacementMap` (Chromium only) or a GLSL refraction shader | One hero moment, never every surface |

Keep text on glass readable and give a solid fallback where `backdrop-filter`
or WebGL is missing.

## Asset guide: free art, 3D and textures

Use the project's own media first. Check each asset's licence before
shipping and credit it where required. Never present a stock asset as the
client's own product.

| Need | Source | Plugs in with |
|---|---|---|
| 3D scene | Spline | `@splinetool/react-spline` or iframe |
| WebGL effect (distortion, glow, liquid) | Unicorn Studio | Its embed script, lazy-loaded |
| Animated illustration, icon, loader | LottieFiles | `@lottiefiles/dotlottie-react` |
| Textures, PBR materials, HDRIs, 3D models | Poly Haven, ambientCG (CC0) | Three.js / React Three Fiber textures |
| Shader ideas | Shadertoy | Study only; most code there is non-commercial |

## Gradient guide

| You want | Use | Needs |
|---|---|---|
| A gradient **video** (pick colours, noise, speed; export MP4 or 4K stills) | Gradient maker at gradients.juangarcia.ch | none; no licence stated, confirm use rights |
| A **live, coded** flowing gradient | ShaderGradient (`@shadergradient/react`) or Paper Shaders (`@paper-design/shaders-react`) | none (npm) |
| A ready WebGL gradient for a hero | AnimatedWebs Gradient Studio | **sign-in** |
| A slow colour drift | Plain CSS (`@property` + animated radial or conic gradients) | none |

A video gives exactly what was designed with no runtime code; live code stays
sharp at any size and can react to the mouse or scroll.

## Rules that always apply

- Call only the tools the request needs, and name them first.
- One design direction, never a blend.
- Check current library docs before writing library code; match the version in `package.json`.
- Respect `prefers-reduced-motion`; pause video, WebGL and animation off screen.
- Keep media light: compress video, lazy-load embeds, add poster frames.
- Before using a `sign-in` tool, tell the user it needs their account.
- When a `connect` or `sign-in` tool would clearly improve the result and
  isn't set up, offer it to the user with what it adds, what it needs and the
  fallback (see "How to use this skill", point 3).
- If a tool fails or is missing, use its fallback and say so in one line.

## Report back

End with: the direction chosen and why (one or two lines), the references
that inspired it, desktop and phone screenshots, any tool that needed a
sign-in and wasn't available, and anything not done or not verified.
