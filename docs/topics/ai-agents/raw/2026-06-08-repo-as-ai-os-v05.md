# Building a Repo as an AI Operating System — v0.5
Date: 2026-06-08
Status: Raw draft — not yet published

---

I've been experimenting with AI on real projects. Not examples, actual work I care about. And things started clicking. I'd have a useful session in Claude, make real progress, build a real point of view. Then I'd open ChatGPT for a second opinion. Then Cursor to build something. Then Codex to review it.

A few weeks in I realized I had no idea where anything lived. The thinking was scattered across six conversation histories I could never search or connect.

I'm not a developer. I'm a product marketer who tests AI on real projects because that's the only way I learn what actually works. And what I needed was a single place where every AI tool could read the same context, write to it, and not make a mess of it.

I asked AI about it. I watched YouTube videos. I landed on GitHub.

It's built for collaboration and documentation, the AI can read markdown natively, and there's version history so nothing gets silently overwritten. You build out a set of instructions and context files, point your AI tools at the repo, and suddenly they're all working from the same source of truth instead of starting from scratch every time.

I'm calling this v0.5 because it's working but not finished. Here's what I've built so far.

---

The two most important files are `AGENTS.md` and `MEMORY.md`. Everything else supports them.

`AGENTS.md` is the front door. Every AI reads this first, every session. It explains who I am, what I'm building, how decisions get made, and where everything lives. Claude, Codex, Cursor, ChatGPT — any AI that connects to the repo reads this file and can get to work without me re-explaining anything.

`MEMORY.md` is the active context. What's in progress, recent decisions, open questions. It's kept short on purpose so it loads fast and stays useful. When something is done it moves to the archive.

The rest of the repo is product thinking in `docs/product/`, build decisions in `docs/build/`, session notes and handoffs in `docs/journal/`, and a topic content pipeline in `docs/topics/` where I build out bodies of work from raw notes to publishable assets.

If you want to start somewhere, start with `AGENTS.md`. Get that right and everything else follows.
