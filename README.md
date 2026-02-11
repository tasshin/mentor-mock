# AI Mentor System - Template

A starter kit for building your own AI mentor system using documents, code, and AI.

## What Is This?

This is a template for creating a **constellation of mentors** — an AI-assisted personal development system that:

- Tracks your growth across multiple life areas
- Invokes different mentor perspectives for different situations
- Maintains conversation logs and patterns over time
- Supports structured SOPs for check-ins, deep dives, and reviews

The system is designed to work with Claude (or another AI assistant) through a `CLAUDE.md` context file that teaches the AI how to work with U specifically.

## How to Use This Template

1. **Fork or copy this repository**
2. **Fill in `CLAUDE.md`** with your personal context, learning style, and preferences
3. **Set up your areas** in `system/areas` — the domains of life U want to grow in
4. **Add your mentors** to `system/mentors` — real people, historical figures, fictional characters, or archetypes
5. **Start using the SOPs** in `system/procedures` — create structured processes for check-ins, deep dives, and reviews
6. **Let it evolve** — the system grows as U use it

### A Note on File Formats

The template files use [org-mode](https://orgmode.org/) (`.org`), but **U don't need to use org-mode**. Markdown, plain text, Notion exports, or whatever format U think in — all work fine. The AI reads them all. What matters is the structure and the concepts, not the file extension.

If U want to convert the included `.org` files to markdown or another format, [pandoc](https://pandoc.org/) makes it easy:

```bash
# Convert a single file
pandoc system/areas.org -o system/areas.md

# Convert all org files to markdown
for f in system/*.org; do pandoc "$f" -o "${f%.org}.md"; done
```

## File Structure

### Root
- **CLAUDE.md** — Context file that teaches your AI assistant how to work with U
- **README.md** — This file

### System (`system/`)
The core of the mentor system:
- **PRINCIPLES** — Guiding principles (multiplicity, rotating perspectives, person-mentor fit, etc.)
- **procedures** — Standard operating procedures for how U do things with your mentor
- **mentor** — The primary Mentor persona definition with role configurations
- **areas** — Your life areas with growth edges, obstacles, and assignments
- **mentors** — Index of your mentors (real, historical, imaginal)
- **conversations** — Log of conversations for continuity across sessions

### Context (`context/`)
Personal context documents:
- **U As A Learner.txt** — How U learn, your preferences and needs (share with teachers/mentors)

### Reference (`reference/`)
Optional background material U can feed to the AI for richer context:
- **The Path of Curiosity.txt** — A book about curiosity, learning, mentors, skill trees, and following your questions ([Tasshin Fogleman](https://tasshin.com), CC BY-NC-SA 4.0). Included as an example of the kind of reference material that deepens person-mentor fit — U can replace it with your own writing, favorite books, or other documents that help the AI understand how U think.

## Core Concepts

### The Rubik's Cube Metaphor
"What would [mentor] do?" — Any hero, historical figure, or abstract concept can serve as a mentor. The system lets U "rotate someone in" and invoke their perspective for any situation.

### Person-Mentor Fit
Like product-market fit, there's a matching problem. The perfect mentor is specifically calibrated to YOU. Generic advice isn't enough; the system must deeply know you.

### Speech Act Tags
The AI tags which role it's speaking from: `[Mentor]`, `[Friend]`, `[Spiritual Teacher]`, `[Boss]`, `[Claude]`, or `[Mentor Name]` for specific mentor perspectives. This makes the rotating perspectives explicit.

### Areas & Assignments
Each life area tracks: Motivation (why it matters), Mentors (who guides U), Growth Edges (where you're developing), Obstacles (what's in the way), and Assignments (what to do next).

## Getting Started

The most important file to fill in first is `CLAUDE.md`. The more context U give, the better the system works. Start with:

1. Who U are and what U care about
2. How U learn (preferences, challenges, what works)
3. Your current life areas and what matters most
4. A few mentors U already look up to

When you're ready, try creating an SOP.
