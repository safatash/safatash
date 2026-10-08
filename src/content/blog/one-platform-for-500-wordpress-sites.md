---
title: How I replaced Freshdesk, InfiniteWP and Jetpack with one AI-powered platform
description: How Nova Support was built, what the AI agent handles by itself, and what still needs a person.
tag: AI · Operations
pubDate: 2026-10-07
---

At Nova Advertising, my team looks after more than 500 client WordPress sites. Every one of them needs small changes all the time: new hours for the holidays, a new staff photo, a phone number in the footer, a page for a new service.

For years we handled all of this with three tools that didn't talk to each other:

- **Freshdesk** for support tickets
- **InfiniteWP** for managing the sites
- **Jetpack** to tell us when a site went down

A simple request meant hopping between all three. Read the ticket in one tool, log in to the site through another, make the change, go back and reply. For a two-minute edit, most of the time went into the switching.

So I built one place to do all of it. We call it **Nova Support**.

## What clients see

Clients sign in with a link sent to their email. There's no password to remember or reset. New people register their email, and our team approves them before they get in.

Once they're in, they send in a request and can see where it stands. They don't have to email back and forth asking whether something got done.

## What happens behind the scenes

This is the part I'm proudest of. Each request goes to an AI agent built on the **Claude API**. The agent is connected to the client's WordPress site. It reads the request, makes the change on the site, and reports back on what it did.

The kind of work that used to sit in a queue, like updating text, swapping an image or adding a page, now gets done by the agent. That frees my team for the jobs that need a person.

> The goal was never to replace my team. It was to stop making skilled people spend their day copying phone numbers into footers.

## Knowing when a site goes down

The last piece was replacing Jetpack's downtime alerts. Nova Support watches every site and alerts us the moment one goes down. Support requests and site health now live in the same place.

## What still needs a person

Bigger jobs still go to a person: redesigns, custom development, and anything that needs judgment about a client's business. AI is very good at the clear, repeatable work, and it frees people up for the work that isn't.

## Why this matters if you own a business

If you own a business, you don't care which tool your web team uses. You care that a change you asked for this morning is live this afternoon, and that someone knows your site is down before your customers do.

That's what one platform gets you: faster turnaround, fewer things slipping through the cracks, and a team that spends its time on work that moves your business forward.

## How it's built

For the technical readers: Nova Support is a Next.js app on Vercel, and the agent runs on the Claude API. I'll go deeper on the architecture in a future post.

If you run an agency or look after a lot of websites and want to talk about building something like this, [get in touch](/#contact).
