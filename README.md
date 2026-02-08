# AI Mentor System - Template

A starter kit for building your own AI mentor system using documents, code, and AI.

## What Is This?

This is a template for creating a **constellation of mentors** — an AI-assisted personal development system that:

- Tracks your growth across multiple life areas
- Invokes different mentor perspectives for different situations
- Maintains conversation logs and patterns over time
- Supports structured SOPs for check-ins, deep dives, and reviews

The system is designed to work with Claude (or another AI assistant) through a `CLAUDE.md` context file that teaches the AI how to work with you specifically.

## How to Use This Template

1. **Fork or copy this repository**
2. **Fill in `CLAUDE.md`** with your personal context, learning style, and preferences
3. **Set up your areas** in `system/areas.org` — the domains of life you want to grow in
4. **Add your mentors** to `system/mentors.org` — real people, historical figures, fictional characters, or archetypes
5. **Start using the SOPs** in `system/procedures.org` — structured processes for check-ins, deep dives, and reviews
6. **Let it evolve** — the system grows as you use it

## File Structure

### Root
- **CLAUDE.md** — Context file that teaches your AI assistant how to work with you
- **README.md** — This file

### System (`system/`)
The core of the mentor system:
- **PRINCIPLES.org** — Guiding principles (multiplicity, rotating perspectives, person-mentor fit, etc.)
- **procedures.org** — Standard operating procedures for check-ins, deep dives, reviews, and conversations
- **mentor.org** — The primary Mentor persona definition with role configurations
- **areas.org** — Your life areas with growth edges, obstacles, and assignments
- **mentors.org** — Index of your mentors (real, historical, imaginal)
- **conversations.org** — Log of conversations for continuity across sessions

### Context (`context/`)
Personal context documents:
- **As A Learner.txt** — How you learn, your preferences and needs (share with teachers/mentors)

## Core Concepts

### The Rubik's Cube Metaphor
"What would [mentor] do?" — Any hero, historical figure, or abstract concept can serve as a mentor. The system lets you "rotate someone in" and invoke their perspective for any situation.

### Person-Mentor Fit
Like product-market fit, there's a matching problem. The perfect mentor is specifically calibrated to YOU. Generic advice isn't enough; the system must deeply know you.

### Speech Act Tags
The AI tags which role it's speaking from: `[Mentor]`, `[Friend]`, `[Spiritual Teacher]`, `[Boss]`, `[Claude]`, or `[Mentor Name]` for specific mentor perspectives. This makes the rotating perspectives explicit.

### Areas & Assignments
Each life area tracks: Motivation (why it matters), Mentors (who guides you), Growth Edges (where you're developing), Obstacles (what's in the way), and Assignments (what to do next).

## Getting Started

The most important file to fill in first is `CLAUDE.md`. The more context you give, the better the system works. Start with:

1. Who you are and what you care about
2. How you learn (preferences, challenges, what works)
3. Your current life areas and what matters most
4. A few mentors you already look up to

Then try running one of the SOPs — the Morning Check-In is a good starting point.
