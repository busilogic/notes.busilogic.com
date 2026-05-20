---
title: "My AI Stunt Double: How I Run Six Engagements Without Losing the Thread"
date: 2026-05-20
description: "A private GitHub repo, a plain-text inbox, and Claude as orchestrator. The personal version of the system I recommend to teams."
draft: true
---

I wrote recently about [using GitHub as your team's AI memory](./github-as-nervous-system). The argument was structural: when context lives in the repo instead of someone's head, it compounds instead of evaporating.

This is the personal version. What I actually use. The system behind the system.

---

## The problem with being a principal consultant

At any given time I'm running five or six concurrent engagements. Each one is at a different point. One is in hypercare. One is mid-migration. One is wrapping up and transitioning support to another consultant. One just started and I'm still learning the landscape.

The switching cost is real. When I'm deep in a cloud migration and I get a message about a completely different client's deployment issue, I have to context-switch fast — different stack, different contacts, different history, different open questions. A to-do app doesn't solve that. Notion doesn't solve that. A good memory helps, but it isn't enough.

What I needed wasn't a better note-taking system. I needed something that holds the operational layer so I can stay at the strategic layer.

## The inbox

Everything starts with a plain-text file called `inbox.md` in a private GitHub repository.

When something comes in — a message, a new action item, a credential I need to store, a reminder I don't want to lose — it goes in the inbox. No formatting, no categorisation, no friction. The only rule is: capture it before it disappears.

```markdown
# Inbox

- Client A: follow up Nathan on subscription access for new consultant
- Client B: check if T&M or drawdown, confirm with PM
- Article idea: write about this system
- New API key for X service: sk-...
```

That's it. It looks like a mess. It's supposed to.

## The orchestrator

Once a day — usually in the morning, sometimes at the end of the day — I tell my AI orchestrator to process the inbox.

It reads every item and routes it:

- Engagement-specific work → the relevant private GitHub issue for that client
- Cross-cutting admin → a dedicated admin issue
- Credentials → the right file in the vault
- Notes → wherever they belong

I don't touch it. I just say "process my inbox" and review what it did.

The routing is the part that matters. Every engagement has its own GitHub issue — a living thread that accumulates context over time. Status updates, blockers, decisions made, next actions. It's not a ticket. It's a running log of everything that's happened and everything that's open.

## GitHub issues as a nervous system

I use private GitHub repositories for this. Not for code. For operational continuity.

Each engagement gets an issue. The issue body is the current state: what's done, what's open, what's blocked. Comments accumulate as things move. The full history is there if I need to reconstruct a timeline or hand over to another consultant.

```
$ gh issue list --repo myorg/engagements --state open

#4  Client D — Azure cost optimisation
#3  Admin & cross-cutting
#2  Side project
#1  Client A — Platform hypercare
```

That single command gives me the complete picture across everything I'm running. No dashboard, no project management tool, no subscription.

The reason GitHub specifically: it's where my work already lives. Commits, PRs, infrastructure changes — it's all there. Keeping the operational layer in the same place means I can link an action item directly to a commit or a PR. Context stays connected.

## The daily view

The issues are the source of truth. But I also maintain a short daily view — a `today.md` that gets refreshed each morning. It's the things I'm actually going to work on today, pulled from the issues, trimmed to what matters right now.

The orchestrator handles the refresh. I read it, adjust if needed, and start working.

## What this actually unlocks

**Nothing drops.** When six things are moving simultaneously, the failure mode isn't being busy — it's forgetting. The inbox catches everything before it disappears into a conversation thread or a mental note I'll lose by afternoon.

**Context accumulates.** Three months into an engagement, the issue history has everything. Why a decision was made. What we tried that didn't work. Who was involved. When I need to brief a new consultant taking over support, the answer is: read the issue.

**I operate at a higher level.** The orchestrator holds the operational layer. I'm not managing my task list — I'm thinking about the client problems. The switching cost drops because the context is already there when I need it.

**It's legible to others.** A colleague can look at an issue and understand where an engagement stands without asking me. That's not just convenient — it's what makes the system durable.

---

## The honest caveat

This system took time to build and it requires a certain disposition — you have to actually capture things, actually process the inbox, actually trust the issues over your memory.

The inbox is only useful if you use it. I've built the habit over months and it's reliable now. In the early days, I'd skip it for a week and pay for it.

The other caveat: I'm not hiding the fact that I use Claude Code as the orchestrator. That's the point. I built a system where AI does the operational routing so I can do the work that requires judgement. Not because it's clever, but because it's the right division of labour.

If you want to build the team version of this — where the same principles apply to an engineering team rather than a solo consultant — [that's here](./github-as-nervous-system).
