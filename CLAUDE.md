# CLAUDE.md – Ink & Thorns

New project started by Tom on 2026-11-20. Display name **Ink & Thorns**; repo `tomandreas/Ink-Thorns` (private), local clone `C:\Users\tom_o\Documents\Repos\Ink-Thorns` (renamed from `Ink&Thorns` on 2026-11-20 because `&` breaks PowerShell paths). Worked on in Claude Code on Tom's PC (Legion; Phanteks has the same layout). Specification written in ChatGPT; source kept unchanged in `docs\`.

## Rules that apply
- General rules for all repos: `C:\Users\tom_o\Documents\Repos\CentralMemories\GENERAL_RULES.md` (loaded through `Repos\CLAUDE.md`). Cross-app status: `CentralMemories\STATUS.md`. Memory: `CentralMemories\GLOBAL_MEMORY.md`, registry entry R-20 in `CentralMemories\PROJECT_REGISTRY.md`, memories in `PROJECT_MEMORIES.md` (PM-IT-..). Where this file and the general rules disagree, this file wins.
- Build only when Tom says "build" (or "bygg"). No application code, scaffolding, dependencies, schemas, migrations, prototypes or deploys before that. Answers in English (GM-001), short, result first, then unintended consequences. Tom is not a developer: steps he must do are numbered with exact text to paste.
- Hosting: Cloudflare (paid Workers plan, GM-021) or Vercel only (GM-012). No new paid AI subscriptions or metered AI APIs without Tom's approval; Tom's ChatGPT and Claude subscriptions are not assumed to give the app API access.
- Never read, print or commit secrets (`.dev.vars`, API keys, tokens, passwords, login emails). Secret names only.
- Source records: `docs\chatgpt-original.md` (Project Goals + Project Instructions) and `docs\chatgpt-first-session.md` (first-session prompt) are immutable, committed 2026-11-20 with no redactions needed. Never edit them; new ChatGPT material goes in a new dated file. They record the starting vision; this file is the current authority.

## Purpose
A private library and reading tracker for Tom's wife (the primary reader, a dark-romance reader), with Tom as second administrator. Physical books only. The app must feel like a luxurious Gothic Romance library rather than a database: on desktop a semi-realistic 2.5D room (shelves, writing desk, laptop), on mobile a dedicated touch interface in the same style. Covers cataloguing with correct editions, search/scan/import, reading status and history, ratings (stars and spice), series, wishlist with secret gift reservations, recommendations from Tom, statistics and push notifications. UI in English. Full text: `docs\chatgpt-original.md`.

## Versions
Git history is the archive (no `versions.json`; same exception as StreamFinder, Heatmap and GearTracker, GM-011; Tom 2026-11-20). The version will be shown in the app and in `/api/health`. No version numbers or scope approved yet.
- **Setup (2026-11-20)**: repo initialised, source docs, this file, `.gitignore`. **No application has been built.**

## How it works
Nothing built yet. No architecture chosen (see Open decisions).

## Decisions (settled, do not re-propose)
- Product requirements: everything listed in `docs\chatgpt-original.md`, Project Instructions section 5 "Settled Functional Decisions" (design, library, book registration, reading information, wishlist, recommendations, accounts and persistence, development). In short:
  - Gothic Romance look (black, burgundy, antique gold, mahogany/walnut, leather, velvet, warm light, subtle animation); one 2.5D desktop room with animated zoom; spines on shelves, a selected book comes forward with cover and details; desk with dynamic stacks of every owned unread book and a separate Currently Reading spot; shelf for owned + read, separate shelf for read but not owned; expanded scrollable shelves for large collections; limited customisation of lighting, theme, decoration.
  - Dedicated mobile interface, bottom navigation, switchable miniature shelves / cover gallery.
  - Separate work, physical edition, ownership, reading status, history, ratings and notes; several editions of one title are not duplicates; history kept when a read book is later bought.
  - Registration: title/author/ISBN search, cover and spine photo recognition (one photo at a time, several books per photo, combined review before saving), manual entry, spreadsheet and reading-app imports, any language, several metadata sources, all metadata correctable, edition and custom cover choice, real spine images where available, user spine photos with auto crop/perspective and manual correction.
  - Notes; stars 0 to 5 and spice 0 to 5 chillies, both in 0.5 steps; completion date with flexible precision; series with order and missing volumes, auto and manual ordering, overridable; advanced search and smart collections.
  - Wishlist: priorities, comments, purchase links, public read-only share link, anonymous gift reservations (optional name, Reserved/Purchased, private management link), visible to Tom only and never to the primary reader (enforced server-side), transfer into the collection.
  - Recommendations from Tom with a message; Accept (to wishlist) or Dismiss; history for the sender; push on new ones.
  - Two individual admin logins, one shared collection, central database and image storage, sync across devices, automatic backups and version history, push for recommendations and collection changes with per-device preferences.
  - Statistics before goals (annual goal optional).
  - Functionality before desktop visuals; priority order in Project Goals section 11 (a priority list, not a version plan).
- Setup decisions (Tom, 2026-11-20, "Accept all" on the conflict review):
  - Communication with Tom in English (GM-001); the spec's own Norwegian default defers to the central rules. UI English.
  - Versioning: git history is the archive (above).
  - "Build" includes the command-line deploy once a deploy target exists (GM-015). The first-session "no deploy" applied to setup only.
  - Design: Ink & Thorns has its own design language (Gothic Romance), an exception to the dark industrial default (GM-006/GM-007).
  - The first-session prompt is kept as its own immutable source file.

## Open decisions (waiting for Tom)
1. First-version scope (a proposal will be given; nothing approved).
2. Tech stack, database, authentication, image storage, deployment topology (within GM-012).
3. Backup, version-history and restore implementation.
4. Book metadata providers (free first).
5. Cover/spine recognition method without paid AI (feasibility unknown).
6. Desktop rendering technology for the 2.5D room.
7. Mobile PWA installation and push strategy.
8. Version numbering (0.x or 1.0 start).

## Unverified (never claim as working)
- Free metadata coverage and quality for non-English editions; series data reliability.
- Whether free/local image recognition can identify covers and several spines from one photo well enough.
- Realistic spine images: no known free source checked.
- Web Push on the primary reader's phone (iPhone needs a Home Screen app, iOS 16.4+, per ST-02; device not known).
- Backup and point-in-time recovery options on Cloudflare (for example D1 Time Travel) not checked for this app.

## To-do (only items Tom asked for)
None. Waiting for Tom's decisions and "build".
