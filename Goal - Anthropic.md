# GOAL.md - Anthropic (2-hour build)


## Standing rules (keep in every GOAL.md)

### Prototype, not demo-as-deliverable
Build a working prototype Ami can walk through in 90 seconds. The deliverable is the prototype. The 90-second demo is only how Ami presents that prototype. Do not treat a demo as the thing you ship.

### UI observation (mandatory)
Public sources only: website screenshots, demo videos (with timestamps), product tours, docs, help center, app-store screenshots, changelog images. Never sign up, create accounts, or log in.

Every GOAL.md must include `## Their UI` before Acceptance criteria, with subsections in this order:
1. Sources
2. Layout
3. Visual style
4. Tone of UI copy
5. The exact screen where my proposed improvement would live
6. Build instruction (match their visual style and terminology so the prototype looks like a feature inside their product)

Be honest: if only marketing illustrations are visible, say "marketing UI only" and infer carefully. If no UI is publicly visible, say so, describe what can be inferred from docs, and default to a clean neutral style.

Writing: simple English. No em dashes or en dashes.

### Phone / mobile UX (mandatory for the prototype)
- Include a proper viewport meta tag so the layout respects phone width.
- Design mobile-first for about 375px width (stack everything vertically).
- No horizontal scroll at phone width.
- Touch-friendly primary actions (about 44px min height / tap target).
- Readable type on a phone (comfortable body size, clear hierarchy).
- No overlays, sticky bars, or modal chrome that clips content or blocks CTAs.
- Good mobile UX overall: one-column flow, large CTAs, thumb-reachable Ship path / Run eval / Send feedback actions.

## Role this GOAL targets
- **Open role (LOCKED):** Applied AI Architect, Startups
- JD: https://job-boards.greenhouse.io/anthropic/jobs/5406982008
- Apply short link (Rémy Olson LinkedIn CTA): https://lnkd.in/g4eh9tK7 → Greenhouse above
- Signal post: Rémy Olson (Applied AI at Anthropic), ~19h before research ET on 2026-09-30: hiring Applied AI Architects for Anthropic's Startups team in San Francisco; work with founders building on Claude (evals, architectures, prototypes); bring learnings back to product and research; wants people who shipped on an LLM API; cares more about technical architecture than the idea; DM note: tell him about something you've built. Profile: https://www.linkedin.com/in/remyolson/ ; post activity: https://www.linkedin.com/feed/update/urn:li:activity:7510766826159738881/
- Location: San Francisco, CA | New York City, NY (Greenhouse). Rémy's post names San Francisco. Hybrid: office at least 25% of the time (JD logistics). Ami: Baltimore MD, open to US relocate / remote; treat SF office presence as the realistic bar for this seat.
- Comp (public): Annual Salary $240,000 to $315,000 USD (Greenhouse JD). Note: JD also says for sales roles the range is OTE; this posting labels the band as Annual Salary.
- Core job (from JD + Rémy): Win trust of founders and engineers as a technical partner helping startups build on the Claude Developer Platform from early product to scale. Architect LLM solutions, win technical evaluations, develop evals, design architectures. Partner with Account Executives through discovery → deployment → expansion. Gather startup build patterns and feed Product / Engineering / research. Travel for workshops and customer sites. Comfortable with Python and common LLM frameworks.
- Bar notes: 3+ years technical customer-facing (Solutions Architect, Sales Engineer, Forward Deployed Engineer, or technical founder with founder-led sales). Startup / high-growth velocity. Builder credibility (SWE or technical founder). Hands-on production LLM apps: context engineering, evaluation frameworks, modern AI architectures. Competitive technical selling. Passion for safe, beneficial AI.
- Fit honesty: This is Applied AI Architect (technical GTM / SA / FDE-adjacent), not a classic AI PM title. Frame the prototype to show Ami's PM craft + shipped-LLM work + eval / architecture taste for founders. Level / title is a stretch vs pure PM path; still a strong Goal Ami can build and pitch.
- Sponsorship: JD explicitly: "We do sponsor visas!" with caveat that Anthropic cannot successfully sponsor every role and every candidate; if they make an offer they will make every reasonable effort and retain immigration counsel. Strong public H-1B LCA history for Anthropic, PBC including Applied AI titles. Favorable for in-country H-1B transfer; still confirm with recruiter on this specific seat.
- Parked (do not build against unless US Startups Architect JD disappears): Applied AI Architect, Startups (London) https://job-boards.greenhouse.io/anthropic/jobs/5432573008 ; Manager of Applied AI Architecture, Startups; Applied AI Claude Evangelist / Technical Evangelist Startup Ecosystem (careers board).

## Company brief (8th-grade English)
Anthropic is a public benefit corporation that builds Claude, a family of frontier AI models, and sells access through consumer Claude products and the Claude Developer Platform (API, Console, docs). Mission: reliable, interpretable, steerable AI that is safe and beneficial. The Applied AI Startups team helps early and growth startups succeed on Claude: architecture, evals, prototypes, and technical wins, then brings field learnings back into product and research. HQ San Francisco. Public product surfaces: anthropic.com, claude.ai / claude.com marketing, platform.claude.com docs, console.anthropic.com (sign-in; never use).

## /goal
Build a working **Claude Startup Architecture Console** for Anthropic's Startups Applied AI seat: load a synthetic early-stage founder who wants their first useful agent on Claude, show a technical discovery stub, an architecture packet (Messages API + tool use + prompt caching + context engineering choices), a founder-facing use-case eval harness that helps win the technical evaluation, a first-deploy checklist, and a one-line Product / research feedback note. Prove Ami can partner like an Applied AI Architect (architecture + evals + prototypes with founders), not a generic Rubric Lens-only hero. Ami must walk through this prototype in 90 seconds.

**Hard product rule:** Do NOT center the hero on a Rubric Lens strip, pass/fail spreadsheet, or graded eval table alone. A compact use-case eval panel is required and OK as part of the architecture packet (JD + Rémy both name evals), but the hero is discovery → Claude architecture → first useful agent path → eval to win the bake-off → feedback to Product / research. Prefer Anthropic / Claude vocabulary throughout.

## Live demo
- Status: built and live (synthetic prototype)
- Link: https://amiteshdwivedijhu-ship-it.github.io/claude-startup-architecture-console/
- What it is: Anthropic-styled Claude Startup Architecture Console (founder discovery → architecture packet → first-deploy path → use-case eval → Product / research feedback)

## Scope (fits 2 hours)
- Synthetic inputs only (no real Anthropic API keys, never sign in to Claude Console or Claude.ai, never create an account, never call live Claude).
- 1 primary path: synthetic founder (example: support triage agent for a B2B SaaS startup) → discovery stub filled → architecture packet recommends Messages API + tools + prompt caching + context pattern → Ami taps Ship first agent path → eval panel shows Claude-favoring cited results for their use case → feedback note ready for Product / research.
- Optional second path: architecture risk (missing eval set or unbounded tool permissions) → gate asks for eval harness or tool-permission tighten before deploy; status stays "Not ready to ship."
- Optional third path: competitive bake-off framing where Claude wins on cited criteria (instruction following / tool reliability / long-context) vs a generic other-model stub; keep other model as "Alt model" without naming competitors if unsure.
- Console must show: founder + use case stub, architecture chips, first-deploy checklist, compact eval panel with citations, human gates (~44px), and a Product / research feedback strip.
- Out of scope: live Claude API, real Console workspaces, production MCP / connector setup, signed-in Claude or Console, Rubric Lens as the only hero, enterprise Strategic / Industries Architect tooling, Rémy DM or Greenhouse apply (outreach is out of this Goal pass).

## Reuse first
- Reuse **evidence / citation packet + human gate** craft from https://amiteshdwivedijhu-ship-it.github.io/ (evidence spans, approve / request / escalate style gates mapped to Ship path / Tighten tools / Need evals / Send feedback).
- Light touch only: pass/fail chips inside the use-case eval panel as secondary. Do NOT force Rubric Lens or a kill-or-ship spreadsheet into the Anthropic hero. Do not pitch Ellipsis as an Anthropic customer.
- Vocabulary to prefer: Claude, Claude Developer Platform, Messages API, tool use, prompt caching, context engineering, evals / evaluation framework, technical evaluation, architecture, first useful agent, prototype, founder, founding engineer, Account Executive, Product / research feedback, Ship path, Workspaces (docs term only). Avoid: scorecard-as-hero, Rubric Lens brand, generic "AI magic" slogans, OpenAI-first framing, cool blue SaaS chrome that fights Anthropic's cream / clay system.

## Their UI

**Honesty note:** Public sources = anthropic.com marketing, Claude product marketing, platform.claude.com docs (Messages, tool use, prompt caching, Run evals), careers. Console at console.anthropic.com requires sign-in; never sign in. No public Startups Applied AI "customer architecture console" was observed. This prototype is **inferred field tooling** an Applied AI Architect would use with a founder, styled to feel Anthropic / Claude. Say when something is inferred. Optional local public HTML captures under `ui/`.

### Sources
- Homepage: https://www.anthropic.com/
- Claude product marketing: https://www.anthropic.com/claude
- Claude Developer Platform docs home / intro: https://platform.claude.com/docs/en/home ; https://platform.claude.com/docs/en/intro
- Docs sections used in vocabulary: Messages API, Tool use, Prompt caching, Run evals, Managed Agents (public nav)
- Advanced tool use engineering note: https://www.anthropic.com/engineering/advanced-tool-use
- Careers: https://www.anthropic.com/careers/jobs
- JD (Startups, SF | NYC): https://job-boards.greenhouse.io/anthropic/jobs/5406982008
- Rémy Olson profile + hiring post: https://www.linkedin.com/in/remyolson/ ; https://www.linkedin.com/feed/update/urn:li:activity:7510766826159738881/
- Optional saved public HTML (not screenshots): `ui/anthropic-home.html`, `ui/claude-platform-docs.html`, `ui/console-landing.html`, `ui/careers.html`, `ui/docs-welcome.html`

### Layout
- Marketing site: warm ivory / cream canvas, dark ink text, restrained clay accent CTAs, serif display + sans UI feel, dark bands for product / model features. Source: https://www.anthropic.com/ ; local `ui/anthropic-home.html`.
- Docs: left nav (Get started, Build, Evaluate and ship, Operate), content column, code samples. Source: https://platform.claude.com/docs/en/home .
- Console: public landing mentions Claude Platform / Developer; signed-in Workspaces / API keys / Playground not observed (never sign in). Source: https://console.anthropic.com/ ; local `ui/console-landing.html`.
- Inferred product surface for this prototype: a **Startups Applied AI Architecture Console** (field tool for Architect + founder, not consumer Claude chat): top = founder / use-case discovery; center = architecture packet + first-deploy checklist; below = compact use-case eval panel; bottom = Product / research feedback strip + gates. (Inferred from JD + Rémy post; not a logged-in screenshot.)

### Visual style
- Colors (from public anthropic.com CSS / design-system reporting, cross-checked in local HTML): canvas ivory `#f0eee6` / `#faf9f5`, card `#faf9f5` / oat `#e3dacc`, ink `#141413`, slate body `#3d3d3a`, muted `#b0aea5` / `#87867f`, clay accent `#d97757` (deep `#c6613f`), optional Claude coral `#cc785c` for primary CTAs if matching Claude product docs.
- Typography: serif for short display titles if easy (or system serif); clean humanist sans for UI labels; monospace for model ids, tool names, citation ids (JetBrains Mono or system mono).
- Density: medium. One founder case open at a time. Architecture chips + checklist + compact eval. Not a dense enterprise spreadsheet.
- Components: rounded cream cards, status pills (Discovery / Architecture ready / Eval running / Ready to ship / Needs evals), clay or coral primary CTAs, citation chips, large touch gates, feedback strip.
- Mode: light cream mode as default (matches public marketing). Optional small dark code strip only for architecture snippet, not the whole page.

### Tone of UI copy
- Applied AI / Claude Platform language: founder, founding engineer, Claude Developer Platform, Messages API, tool use, prompt caching, context engineering, evaluation framework, technical evaluation, architecture, first useful agent, prototype, Ship path, Product feedback, research feedback.
- JD / Rémy words to reuse: win technical evaluations, develop evals, design architectures, build on Claude, bring learnings back to product and research, shipped on an LLM API, technical architecture over idea.
- Calm, precise, builder-first. No growth-hack hype. No unsafe autonomy claims. Prefer "human gate before deploy" framing that fits Anthropic's safety posture.

### The exact screen where my proposed improvement would live
- An inferred **Startups Applied AI working session** screen: after an Account Executive (or inbound founder) brings a startup into technical discovery, before they lock architecture and before they declare a technical evaluation win. This is the surface the Applied AI Architect, Startups seat is hired to own (JD: discovery through deployment; evals + architectures; feedback to Product / Engineering).

### Build instruction
- Match Anthropic closely enough that the prototype feels like internal Startups field tooling: cream / ivory paper, ink text, clay / coral primary CTAs, muted secondary labels, monospace for API / tool ids, rounded cards, citation chips, large Ship / Tighten / Need evals / Send feedback CTAs.
- Use their terminology: Claude, Claude Developer Platform, Messages API, tool use, prompt caching, context engineering, evals, technical evaluation, architecture, first useful agent, founder, Product / research feedback.
- Walk top-to-bottom (phone) or left-to-right (desktop): discovery → architecture packet → first-deploy checklist → compact eval → feedback strip. Keep eval chips secondary to architecture + deploy path.
- Phone / mobile UX is mandatory: viewport meta, ~375px stack, no horizontal scroll, ~44px tap targets, readable type, no overlay clipping CTAs.
- Rejected pattern: do not rebuild a Rubric Lens / scorecard demo as the only hero. Do not clone consumer Claude chat. Do not build enterprise Strategic Architect account planning. Do not sign in to Console.

## Acceptance criteria (must work when Ami demos the prototype in 90 seconds)
1. Load a synthetic founder / use-case stub → show company stub, agent goal, and at least 3 architecture chips (example: Messages API, tool use, prompt caching or context engineering pattern).
2. Human gate lets Ami pick Ship first agent path, Tighten tool permissions, Need evals before deploy, or Send Product / research feedback. Primary CTAs are touch-friendly (~44px).
3. Ship path updates status to Ready to ship (or Deploy checklist complete) and shows compact eval panel with at least 2 cited findings favoring Claude for this use case (or an honest "eval incomplete" if on the Need evals path).
4. Optional Need evals / Tighten path keeps status blocked with a clear reason and listed missing items.
5. Hero is the Claude Startup Architecture Console (discovery → architecture → first useful agent → eval → feedback), not a pass/fail spreadsheet or Rubric Lens strip alone.
6. Opens cleanly on a phone-width viewport (~375px) with viewport meta, vertical stack, no horizontal scroll, ~44px touch targets, readable type, and no overlays clipping content.
7. Walkthrough proves discovery → architecture → deploy path → eval → Product / research feedback in ~90 seconds.

## What the 90-second walkthrough proves about THEIR problem
Anthropic's Startups Applied AI Architects win trust with founders by helping them build on the Claude Developer Platform: architectures, evals, and prototypes, then feeding field learnings back to product and research (https://job-boards.greenhouse.io/anthropic/jobs/5406982008 ; Rémy Olson hiring post). Walking through this prototype shows Ami can run a founder-facing session that turns a vague "we want an agent" into a Claude architecture packet, a first useful agent path, a use-case eval that supports the technical win, and a concrete feedback note for Product / research, which is the job, not a generic eval demo.

## TIMEBOX
If the prototype is not walkthrough-ready at 2 hours: LIGHT pitch fallback = open citation + human-gate craft from https://amiteshdwivedijhu-ship-it.github.io/ + 2 mapping lines:
1) "Your Startups Applied AI Architect seat helps founders ship on Claude with solid architectures, evals, and prototypes, then brings learnings back to product and research."
2) "The 2-hour extension is an Anthropic-styled Claude Startup Architecture Console: discovery → architecture packet → first useful agent path → use-case eval → Product / research feedback."
Do not fall back to Rubric Lens alone as the story. Do not pivot the Goal to London Startups Architect or Evangelist seats unless the US Startups Architect JD is gone.
