---
title: "The Business Risk of Every Technical Departure"
date: 2026-04-10
description: "By the time you realise it's an operational risk, the knowledge is already gone."
---

When an engineer or a technical resource announces they're leaving, most people see it as an HR problem. 
Find a replacement, arrange a handover, done. Then, when 3 months later, something breaks that only the previous person knew how to handle, the team quietly scrambles to figure it out.

I've managed enough of these transitions in various capacities (as a team lead, as the consultant to fix the aftermath, and as the engagement owner) to know that the risk is always underestimated and preventable. This is my playbook.

## The timeline shapes your risk

First, understand how long you have. 

In Australia, standard notice periods are four weeks. In India, it's typically two to three months — sometimes longer for senior engineers. 

With a month runway, you're doing triage. Identify the highest-risk knowledge gaps and focus there. You're optimising for continuity of the most critical functions, accepting that comprehensive documentation may not be possible.

With three months, a proper overlap is possible. The outgoing engineer can first lead, hand over gradually, then support as the incoming engineer takes the reins. You surface the edge cases — the things that only come up once a quarter but will break something important when they do.


## Start the moment you know

Second, the day someone announces they're leaving is the day the handover starts. 

A simple question to ask yourself: *What are the 3 things that would go wrong in the next six months if you just disappeared today?* 
Most can answer this in ten minutes. That's your risk register.

From there, the handover should map out what the incoming engineer needs to know, how critical it is, and how complex the knowledge is to transfer. 

Some things are quick like credentials, access, runbooks. Others take weeks of working alongside someone — client relationship dynamics, why a decision was made two years ago, the unwritten rules of how a particular stakeholder communicates.

The complex, high-criticality items need calendar time immediately. The rest get documented and checked off. Your job is to make sure this mapping happens in week one, not week three.

## The tribal knowledge problem is your biggest risk

Tribal knowledge is information that lives in someone's head rather than in any system. This is the most dangerous category of a handover because it's invisible until it's gone.

I see it as three forms:

**Relationship knowledge** — who the real decision maker is (not the org chart one), who to call when the official channel is blocked, which stakeholder needs to be kept informed even when they're not officially involved. New engineers can have the technical skills and still fail engagements because they don't understand the nuances.

**Context knowledge** — why the system is the way it is. What was tried and didn't work. What the constraints were that shaped the architecture. Without this, incoming engineers make locally rational decisions that are globally wrong.

**Operational knowledge** — the things you just know after running something for a while. The deployment that needs to happen in a particular order. The check that should be run before the monthly maintenance window. The thing that looks like an error but isn't.

The way to surface tribal knowledge before it walks out the door: run incident simulations. 
Give the incoming engineer a scenario — something that has actually gone wrong — and watch how they'd handle it. The gaps in their response show you exactly what hasn't been transferred yet. Do this early enough that you have time to fill the gaps.

## What good looks like

Regardless of runway time, a well-run handover follows a clear structure.

**Phase one: shadow and document.** The outgoing engineer leads everything. The incoming engineer observes, asks questions, and writes. Every meeting, every client interaction, every deployment. By the end you have a baseline knowledge base and the incoming engineer has context.

**Phase two: lead together.** They share responsibility. The incoming engineer starts leading client interactions and technical decisions, with the outgoing engineer present. The outgoing engineer's job is to let the new person make recoverable mistakes, and to intervene on the ones that aren't. This is where the real knowledge transfer happens — not through documents, but through doing.

**Phase three: independent with support.** The incoming engineer leads. The outgoing engineer is available for questions but not present in meetings. 


## Handovers reveal your real operational risk

Here's the uncomfortable thing a handover will show you: the state of your team's documentation is usually worse than you thought.

Every handover is an audit of operational maturity. How long does it take to onboard someone new? 

What questions does the incoming engineer ask that no document can answer? Those are your documentation gaps. 

What breaks in the first month of their independence? Those are your brittleness points.


## What this means for how you lead

Handle departures by treating them as a forcing function for operational health, not a crisis to manage. 
Make documentation a standard part of delivery, not an afterthought.

And if you're regularly losing knowledge when people leave, the issue isn't the departing engineer. It's how the team has been run. The handover is just the moment it becomes visible.
