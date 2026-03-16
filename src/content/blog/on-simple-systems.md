---
title: On Simple Systems
date: 2026-03-10
description: Why I keep coming back to boring, predictable tools.
---

There's a line I keep returning to from Rich Hickey: *"Simple is not easy."* Simplicity
is a property of the thing itself — few moving parts, limited scope, clear contracts.
Easy is a property of the relationship between you and the thing.

The two are often in tension, and we usually optimize for the wrong one.

## The seduction of cleverness

Early in my career I loved clever code. Terse, abstract, exploiting every language
feature available. It felt like craftsmanship. Looking at it now, I see what it really
was: complexity dressed up as sophistication.

The problem with clever code is that you can only read it in the right state of mind.
At 9am, well-rested, with full context. Not at 11pm during an incident.

## What I reach for instead

These days I ask a different question before I write anything: *"What is the simplest
thing that could possibly work?"*

Sometimes the answer is boring. A flat list instead of a tree. A cron job instead of
an event bus. A SQL query instead of a cache layer. I've learned to love boring answers.

## The hidden cost of abstraction

Every abstraction you add is a bet that it will be used enough to justify its cognitive
overhead. Most of the time that bet loses. You end up with a generic framework for a
problem that only ever had one instance.

Prefer concrete over abstract, specific over general, until the generalization earns itself
through repeated, identical use.

---

Simple systems are easier to debug, easier to hand off, and easier to delete when they're
no longer needed. That last one matters more than people admit.
