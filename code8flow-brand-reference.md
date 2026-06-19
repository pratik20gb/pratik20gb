# Code8Flow — Brand & Content Reference

A reference document for generating consistent brand assets: websites, videos, thumbnails, social posts, and marketing material for Code8Flow. Paste this whole file into Claude (or any AI tool) before asking it to design or write anything for the project.

---

## 1. Product Identity

**Name:** Code8Flow
**Category:** Project management SaaS (Jira-style workspace/board/task tool)
**Tagline options:**
- "Where work flows."
- "Project management, engineered properly."
- "Built like the tools you already trust."

**One-line description:**
Code8Flow is a full-stack project management platform with workspaces, boards, and tasks — built on a production-grade Java Spring Boot backend with JWT auth, Redis caching, async event processing, and a React frontend.

**Positioning:** Code8Flow is presented as a polished, professional SaaS product. Avoid any language suggesting it's a learning project, tutorial, student build, or "MVP" — public-facing copy should read like an established or seriously emerging product.

---

## 2. Target Audience (for content tone)

```
Primary  → Small engineering/product teams evaluating a lightweight
           Jira alternative
Secondary → Developers and recruiters viewing the GitHub repo /
            portfolio (SDE-1 hiring context)
Tertiary  → Developer audience on YouTube/X watching build content
```

Two different tones are needed depending on the channel:
- **Product-facing content** (landing page, app screenshots, demo videos): confident, professional, benefit-driven, zero mention of "learning."
- **Build-in-public content** (YouTube streams, X posts, dev blog): technical, transparent, shows real debugging — this is where the engineering journey is fine to reference.

Never mix these two tones in the same asset.

---

## 3. Visual Identity

### Color Palette

**Brand mark palette (logo, hero moments, premium touchpoints)**
```
Background    Near-black      #0A0A0A   — logo background, hero sections,
                                          premium/launch moments
Gold gradient (back square)
  highlight   #FFFFFF → #FFF3CC → #D9A53D → #9A7325 → #6E4F15
Gold gradient (front square)
  highlight   #FFFFFF → #FFF8DE → #E8B84B → #B8862E → #8A621F
```
The logo mark is two overlapping hollow squares (rounded corners) with a
gold metallic stroke gradient — bright white-gold catching the top-left
corner of each square, fading to deeper bronze toward the bottom-right,
simulating light reflecting off a beveled metal edge. Lives on a
near-black (#0A0A0A) background. This is the primary brand mark and
should anchor logo usage, splash/launch screens, and premium marketing
moments (hero sections, video intros, merch).

**Product UI palette (app interface, day-to-day product surfaces)**
```
Primary (Brand)
  Deep Indigo     #4F46E5   — primary actions, links, in-app accents
  Indigo Dark     #3730A3   — hover states, headers

Secondary
  Teal Accent     #0D9488   — success states, secondary CTAs
  Amber           #D97706   — warnings, priority HIGH/URGENT badges

Neutrals
  Ink             #111827   — primary text
  Slate           #4B5563   — secondary text
  Mist            #F3F4F6   — backgrounds, cards
  White           #FFFFFF   — base background

Status Colors (match TaskStatus enum)
  TODO            #94A3B8   (slate gray)
  IN_PROGRESS     #3B82F6   (blue)
  IN_REVIEW       #D97706   (amber)
  DONE            #10B981   (green)

Priority Colors (match Priority enum)
  LOW             #94A3B8
  MEDIUM          #3B82F6
  HIGH            #D97706
  URGENT          #DC2626
```

**How the two palettes coexist:** the black/gold palette is for brand
identity and marketing — logo, landing page hero, launch video, social
profile imagery. The indigo/teal palette is for the actual product
interface — buttons, status badges, in-app accents. Think of it like
how a premium product's packaging can be black-and-gold while the
device/app interior uses a completely different, more functional color
system. Never use the gold gradient for in-app UI elements (buttons,
badges) — it does not have the contrast/accessibility profile for
repeated UI use. Never use flat indigo/teal for the logo mark itself —
the gold-on-black is the brand mark, full stop.

### Typography

```
Headings  → Inter (Bold/Semibold) or Geist
Body      → Inter (Regular)
Code/UI   → JetBrains Mono — use for any code snippets shown in
            marketing material (reinforces the engineering credibility)
```

### Logo — finalized

```
Mark      → two overlapping hollow squares (rounded corners, ~13px
            radius at 80px square size), offset diagonally so they
            intersect in the lower-right quadrant of the first square
Stroke    → gold metallic gradient, ~4-5px width at full size
            white-gold highlight at top-left corner, fading through
            amber to deep bronze at bottom-right corner of each square
Background → near-black (#0A0A0A), always — this mark is not designed
            for use on white/light backgrounds
Wordmark   → "code8flow" (lowercase, no space) in a gold gradient,
            paired to the right of the icon for the full lockup
```

**Why this direction:** the two-square motif reads as kanban cards in
motion (literal product connection — boards and tasks), while the
hollow/outline treatment with metallic gold keeps it premium rather
than flat/generic-SaaS. Confirmed legible down to 16-32px (favicon/app
icon scale) — the overlap and gradient remain readable at that size.

**Asset files (reference):**
```
code8flow-icon.svg            — icon only, transparent background
code8flow-icon-on-black.svg   — icon with #0A0A0A background baked in
                                 (use this for app icons, social avatars)
code8flow-favicon.svg         — simplified/optimized for 16-32px display
code8flow-wordmark-lockup.svg — icon + "code8flow" wordmark, horizontal
```

**Usage rules:**
```
✅ Always on black/near-black background
✅ Icon-only version for square contexts (favicon, app icon, social avatar)
✅ Wordmark lockup for horizontal contexts (website header, video outro,
   email signature)
❌ Never recolor the gradient to indigo/teal — gold-on-black is the
   fixed brand mark
❌ Never place on light/white backgrounds — contrast and shine effect
   both fail
❌ Never stretch non-uniformly — always scale the icon proportionally
```

### Imagery style

```
Product screenshots → clean browser mockups, generous white space,
                       soft drop shadows, rounded corners (8-12px)
Illustrations        → if used, flat geometric style, limited palette
                       (primary + one accent), no stock-photo people
Code snippets         → dark theme (e.g. One Dark Pro / Dracula-style),
                       used sparingly in build-in-public content only
```

---

## 4. Voice & Tone Guidelines

### Product copy (website, app, demo videos)
```
✅ Direct, confident, benefit-led
✅ Short sentences, active voice
✅ "Move work forward" not "Workflow management capabilities enabled"
❌ No hedging language ("might help", "could potentially")
❌ No mention of being a learning/practice/portfolio project
❌ No apologetic tone about features being incomplete
```

Example good copy:
> "Workspaces, boards, and tasks — without the bloat. Code8Flow keeps your team's work visible and moving, backed by infrastructure built for scale from day one."

Example bad copy (avoid this tone):
> "This is my project where I'm learning Spring Boot and trying to build something like Jira!"

### Build-in-public / developer content (YouTube, X, dev blog)
```
✅ Technical specificity — real numbers, real errors, real fixes
✅ Show the debugging, not just the success
✅ Confident but honest ("hit a tricky AWS signature bug, here's the fix")
❌ Don't fabricate difficulty or oversell minor issues
❌ Don't undersell real wins with false modesty
```

---

## 5. Architecture Talking Points (for technical content/videos)

Use these when generating technical marketing content, dev videos, or technical blog posts — they double as credibility signals for both users and recruiters.

```
Backend       → Java 21, Spring Boot 4, layered architecture
                (Controller → Service → Repository)
Auth          → JWT with access + refresh token rotation, BCrypt hashing
Database      → PostgreSQL with Flyway-versioned migrations
Caching       → Redis, ~15x read latency improvement on cached endpoints
File storage  → AWS S3 with pre-signed URLs (files never touch the
                app server)
Async/Events  → Kafka-based event-driven notifications (Phase 5+)
Frontend      → React 18 + TypeScript
DevOps        → Docker Compose for local dev, GitHub Actions CI/CD
Observability → Prometheus + Grafana (planned)
```

---

## 6. Content Pillars (for ongoing video/post planning)

```
1. Product demos        → screen recordings of actual app usage,
                           workspace/board/task flows
2. Engineering deep-dives → "How JWT auth works", "Why we use
                            pre-signed URLs for S3", etc.
3. Build-in-public logs  → stream recaps, bug-fix stories, phase
                            completions
4. Comparison content    → Code8Flow vs. existing tools (feature
                            angle, not disparaging competitors)
```

---

## 7. Naming Conventions

```
Product name      → Code8Flow (always one word, capital C and F)
Repo/package name  → code8flow / com.cod8flow.cod8flow (internal only,
                     never shown in product-facing copy)
Domain workspace   → "Workspace" → "Board" → "Task" (always this
                     hierarchy and these exact terms in UI copy)
```

---

## 8. What NOT to include in any generated asset

```
❌ "Tutorial", "learning project", "practice app", "student build"
❌ Screenshots showing IDE, terminal, or raw code in product marketing
   (those belong only in build-in-public/developer content)
❌ Comparisons that mention specific competitor pricing or disparage
   competitors directly
❌ Placeholder Lorem Ipsum text in any final deliverable
❌ Generic stock SaaS imagery (laptop-on-desk photos, generic
   handshake images, etc.)
```

---

## 9. Quick-Use Prompt Template

When asking Claude (or another AI) to generate a new asset, prepend this:

> "Using the Code8Flow brand reference [paste this doc], create a [website hero section / video script / thumbnail concept / social post] for [specific purpose]. Match the visual identity, voice, and positioning exactly as specified — this is product-facing content unless I say otherwise."

For build-in-public content specifically, add:

> "This is build-in-public developer content, not product marketing — use the developer voice/tone guidelines instead of the product copy guidelines."

---

## 10. Open Items to Define Later

```
☑ Final logo file (SVG) — DONE, see asset files listed in section 3
☐ Confirmed primary domain name
☐ Social handles (X, YouTube channel name)
☐ App screenshots library (capture once Phase 7 frontend is live)
☐ Demo video script (capture once core flows are stable)
☐ Production wordmark font (current lockup uses placeholder Arial bold —
  swap for a proper typeface, e.g. a geometric sans, before final use)
```
