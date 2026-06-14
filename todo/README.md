# 🧭 Daily To-Do / Command Center System

A lightweight, Claude-driven productivity system. The **data is plain Markdown** (renders as a real visual anywhere — Obsidian, Google Drive, your phone) and **Claude is the interface** (ask it where you are, what's next, mark things done).

## How it works

```
todo/
  dashboard.md        ← THE document. Your "where am I?" view. Refreshed each morning.
  inbox.md            ← Quick capture. Triaged every morning.
  areas/              ← One file per thing you're working on (project / client / life area)
    _TEMPLATE.md      ← Copy this to add a new area
    example-area.md   ← Sample — delete once you add real ones
  daily/              ← One file per day: morning plan + end-of-day log
    2026-06-14.md
  templates/          ← Templates for daily files and the weekly review
  weekly/             ← Weekly review notes (created by /weekly-review)
```

**The flow:**
- **Areas** are the source of truth — each has a status, progress, and a single *next action*.
- The **dashboard** is a generated snapshot that rolls all areas + today's plan into one visual page.
- The **daily file** is what you commit to *today*.
- The **inbox** catches stray thoughts so you never break flow to organize.

## Talk to it (works in the Claude app, web, and CLI — equally)

| Command | What it does |
|---------|--------------|
| `/morning` | Triages inbox, builds today's plan, refreshes the dashboard, greets you |
| `/status`  | "Where am I?" — snapshot across all areas + today |
| `/next`    | Just the single next thing to do |
| `/done <thing>` | Marks it complete, advances the area, updates the dashboard |
| `/capture <thought>` | Drops something into the inbox without stopping to organize |
| `/weekly-review` | Zoom out, review all areas, set next week's focus |

You can also just talk normally — "what's slipping?", "move X to next week", "add a new area for the Y project" — Claude reads and edits these files directly.

## Living in your local KB (Google Drive synced)

This works great as a folder inside your Drive-synced KB:
1. Copy both the **`todo/`** folder and the **`.claude/`** folder into your KB folder.
2. Open a local Claude Code session pointed at that folder (`claude` in the terminal there, or open the folder in the desktop app).
3. The Markdown renders in Obsidian/Drive; Drive handles backup + sync across devices; Claude gives you the `/` commands.

> The `.claude/` folder carries the slash commands, so they travel with the system.

## Customizing

- **Add an area:** copy `areas/_TEMPLATE.md` → `areas/<name>.md`, or ask Claude to.
- **Add/edit a command:** they're just Markdown files in `.claude/commands/`. Ask Claude to create one (e.g. `/evening` for a shutdown routine).
- **Auto-greet on open (optional):** a `SessionStart` hook can show your dashboard automatically every time you open the folder. Ask Claude to add it and approve the change, or add it yourself to `.claude/settings.json`.

## Conventions (so Claude stays consistent)
- Status: 🔴 urgent/blocked · 🟡 needs attention · 🟢 on track · ✅ done · ⚪ not started
- Progress bars: `▓▓▓░░ 60%`
- Each area always keeps exactly one **➡️ Next action** filled in — that's what powers the dashboard.
