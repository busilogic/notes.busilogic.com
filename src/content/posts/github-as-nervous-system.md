---
title: "GitHub as Your Team's AI Memory"
date: 2026-04-24
description: "The difference between AI that helps individuals and AI that helps teams is shared infrastructure."
---

Most teams have adopted AI tools. Most people want to be productive and focus on higher order work. 
However, how they use these tools varies widely. Everyone is figuring it out as they go along. Due to the frontier nature of the AI cycle, every engineer is at different points of AI maturity.

## Context is everything

LLMs are currently mature enough that if you provide enough context, you can get a decent result to a decent question.

Prompt engineering has grown into context engineering. Give the LLM enough context, pre-requisites and guardrails to give a better answer. The aim is to generalise context — some of it applies everywhere, some applies only to the current question.
For example, I restrict every question to a topic. And every question has some pre-requisites to take into account.

## How teams are trying to solve it

Different workarounds have popped up. One method is pasting in chunks of documentation. Another is notes that are copied in at the start of each session. Another is separation of concerns by folders, restricting the AI to only that context.

These are individuals' habits with various results, but none of it is team infrastructure. When the engineer leaves, the system leaves with them.

This is the same tribal knowledge problem I see in handovers — knowledge that lives in a person's head instead of a shared system. 

## The fix is standardisation

When I started running AI-assisted engagements seriously, I made the same mistakes. I had to stop thinking about AI context as a prompt problem and start thinking about it as an infrastructure problem. I started using GitHub as the team's memory.

I started a standard of sorts. Every engagement gets the same structure from day one. 
- A `deliverables/` folder for outputs 
- `notes/` for working material 
- `memory/` for what the AI needs to know (e.g. decisions made, constraints, architecture, client context) 
- A single context file at the root that wires it all together and gets read automatically when a session opens.

No re-establishing context. No "remind me where we were." The AI picks up where the last session left off because the context is persistent and shared.

Engineers left to their own devices will each invent their own system. But none of it is transferable, none of it compounds, and none of it survives a team change.

Getting AI to actually deliver productivity gains at a team level isn't a tooling decision — it's a standards decision. Someone with authority needs to say: this is how we structure context for AI-assisted work, and it lives in the repo alongside the code.

That's a five-minute decision that can have compounding returns. Teams that do it early build on each session and don't have to keep starting over.

## What this unlocked for me

Once context lives in the repo, three things happen.

**Continuity across sessions.** Work builds on itself instead of resetting. The productivity gains people expected from AI actually start materialising.

**Decisions as artefacts.** When a stakeholder asks why something was built a certain way, the answer is in the commit history — not reconstructed from memory six months later.

**Handovers that actually work.** The repo is the handoff. The context is there. A new engineer or a new AI session inherits everything without extraction.

