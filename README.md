# Sideline — team platform for Işık Chargers

> The all-in-one digital home of the Işık University Chargers American football team, used daily by the whole roster and coaching staff.

**Web app (mobile-first)** · [chargers.melberlabs.com](https://chargers.melberlabs.com) · Designed, built and operated by [İbrahim Melikşah Köse](https://github.com/meliksahkose), team captain 2023–2026 and current linebacker coach

## What it does
- **Practice schedule and attendance**: players report availability, and coaches take roll in seconds.
- **Animated 11v11 playbook** for offence and defence.
- **Learning centre with exams**, so coaches can check that players know their assignments.
- **Film room, depth chart and tasks** for game preparation.
- **XP and progression ("Locker")** plus a Retro Bowl-style mini game with live duels, to keep players engaged between practices.
- **Roles**: player, coach, head coach and admin. Invite links, Google sign-in and an approval queue.

Clubs usually pay for this kind of tooling in commercial products such as Hudl. Sideline gives a university club these capabilities on its own infrastructure.

## Engineering decisions
- **Server-validated game engine.** Mini-game inputs are replayed and validated on the server with a deterministic engine, and replay tests confirm identical outcomes.
- **End-to-end tested.** Playwright covers sign-in, invite, approval and role permissions across every page.
- **Stack:** Next.js 16 · React 19 · Tailwind v4 · Better Auth (Google) · Drizzle ORM + PostgreSQL · Docker on a self-managed Linux server · GitHub Actions.

---
<sub>Source code is private (the code and content belong to the club). Happy to demo it in an interview: meliksah.kose1@hotmail.com</sub>
