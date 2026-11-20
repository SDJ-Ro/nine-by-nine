# Nine by Nine: Sudoku Duels — Progress

**Current Phase:** Phase 0 (Setup)
**Team:** 2 beginners (split & teach: Go backend / React + TS frontend)

## Locked Decisions
- **Scope:** Classic 9x9 only (no 6x6, 16x16, Killer, or other grid variants).
- **Stack:** Go (modular monolith), React + TypeScript (Vite), Zustand, PostgreSQL, WebSockets (gameplay) + REST (everything else), Docker. Redis deferred.
- **Core Rules:** Server-authoritative (solution never sent to client), Room-as-actor (1 goroutine/room), append-only event log.
- **UI & VFX:** Plain grid first with CSS variables + Event Bus; Sketchbook/watercolor VFX added last as a deletable layer.
- **Daily Reset:** Midnight Sri Lanka time (UTC+5:30 / 18:30 UTC), local countdown, archive playable for reduced points (no streak/leaderboard effect).
- **Guests:** 30-day sliding cookie + `guests` table; merge daily solves & streak only on Google OAuth signup (account wins conflicts).
- **Hosting (Zero Budget):** Cloudflare Pages (web) + Oracle Always Free VM (Go + Postgres).
- **Git Rule:** Never push directly to `main` — always use branches + Pull Requests.

## Roadmap
- [ ] **Phase 0:** Setup (repo, folders, tools, first PRs)
- [ ] **Phase 1:** 9x9 Core (Go) + Plain 9x9 Grid (React)
- [ ] **Phase 2:** Connect API + Postgres (Solo Play)
- [ ] **Modules:** Daily & Archive | 1v1 Duels | Co-op | Accounts & Guest Merge | Bots/Ghosts | Tournaments | Sketchbook VFX | Deploy

## Done So Far
- [x] GitHub repo created (`SDJ-Ro/nine-by-nine`) & collaborator added
- [x] Local repo linked & `setup/init-docs` branch created
- [x] `docs/PROGRESS.md` and `.gitignore` created