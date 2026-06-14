# 🚀 Setup — Daily To-Do / Command Center

You're moving this into your **local KB folder** (the one synced to Google Drive).
Pick whichever path is easiest. Either way you end up with two folders — `todo/`
and `.claude/` — inside your KB folder.

---

## Option A — Use the bundle I sent you (simplest)

1. Save **`todo-system.zip`** into your KB folder (e.g. `…/Google Drive/KB/`).
2. Unzip it *there*. You should now see:
   ```
   KB/
     todo/
     .claude/
     SETUP.md
   ```
   > `.claude` starts with a dot, so it may be hidden. On Mac press **⌘ + Shift + .**
   > in Finder to show hidden files and confirm it's there.
3. Open a Claude Code session pointed at the KB folder:
   - **Terminal:** `cd "<path to your KB folder>"` then run `claude`
   - **Desktop app:** open that folder as the project.
4. Type `/status` — if Claude reports your dashboard, it's wired up correctly. 🎉

---

## Option B — Pull it from git instead

If you'd rather track it in git:
```bash
cd "<your KB folder>"
git clone <your repo url> .            # or copy the todo/ and .claude/ folders in
git checkout claude/daily-todo-system-htysz1
```

---

## First run

1. `/morning` — sets up today and walks you through your first plan.
2. Replace `todo/areas/example-area.md` with a real area, or just tell Claude
   "add an area for <project>".
3. Drop stray thoughts anytime with `/capture <thing>`.

## Daily commands
`/morning` · `/status` · `/next` · `/done <thing>` · `/capture <thing>` · `/weekly-review`

## Notes
- Google Drive handles backup + sync across your devices automatically.
- The Markdown renders as a visual in Obsidian, Drive preview, and on your phone.
- Want the dashboard to show automatically every time you open the folder? Ask
  Claude in your new session to "add the SessionStart auto-greet hook" and approve it.
- Full reference: `todo/README.md`.
