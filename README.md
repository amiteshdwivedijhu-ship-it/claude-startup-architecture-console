# Claude Startup Architecture Console

Working prototype for the Applied AI Architect, Startups seat at Anthropic: a founder-facing working session that turns "we want an agent" into a Claude architecture packet, a first useful agent path, a use-case eval that supports the technical win, and one line of feedback for Product / research.

## What it demonstrates

The JD asks for architects who win technical evaluations, develop evals, design architectures, and bring field learnings back to product and research. This console walks a synthetic founder (Maya Chen, founding engineer at Kitepath, a B2B SaaS) through:

1. Discovery: company stub, agent goal (support triage, draft replies, human approves), constraints
2. Architecture packet: Messages API + tool use loop, prompt caching, context engineering, human gate before deploy, with an illustrative snippet and citations to public Claude Developer Platform docs
3. First-deploy checklist: one tool, draft-only week 1, prompt caching, eval set, read-only permissions, budget cap
4. Use-case eval: compact cited findings (instruction following, tool reliability, long-context cost) from a 20-ticket synthetic eval set
5. Human gates: Ship first agent path, Tighten tool permissions, Need evals before deploy, Send Product / research feedback
6. Product / research feedback strip: one field-learning line, sent with one tap

## 90-second walkthrough

1. Load: founder + use case stub, architecture packet with 4 chips, deploy checklist (2 open), eval panel with 3 cited findings
2. Tap "Ship first agent path" → status flips to Ready to ship, checklist completes, eval verdict stands
3. Reset, tap "Tighten tool permissions" → blocked with reason and missing items
4. Reset, tap "Need evals before deploy" → auto-reply tool blocked with its own missing eval set
5. Tap "Send Product / research feedback" → one line logged to the field learnings loop

## Status

Synthetic data only. No live Claude API calls, no accounts, no Console sign-in, no real Kitepath data. Not affiliated with Anthropic. The console surface is an inferred field-tooling surface built from the public JD and Claude Developer Platform docs language, not an observed product screen. Eval results are synthetic; citations link to public docs.

Live at https://amiteshdwivedijhu-ship-it.github.io/claude-startup-architecture-console/