# File-Access Skill for OpenClaw — Free Sample

A hardened file-access skill for personal AI agents, plus a one-page
token-burn checklist. Free, open, and yours to use and change.

## What the file-access skill does

It lets your agent work with everyday documents — find a file, read it,
summarize it, copy it into a work folder — without giving it the run of
the whole machine:

- **Allowlist only.** The agent can see at most 10 folders you name in
  advance. Everything outside them is invisible to the skill.
- **Copies and new files only.** It never deletes, moves, or overwrites
  an existing file.
- **Size caps.** 2 MB per file read, 20 files per run, 10 MB total read
  per run; copies capped at 20 MB per file, 5 per run.
- **Credential ban.** It never opens key files, password vaults, browser
  profile folders, or anything named like `*secret*`, `*token*`, `*key*`,
  `.env`, or `credentials*`.
- **Audit log.** Every action is appended to `agent-file-log.md` in the
  work folder: time, action, path, size, result — so you can check what
  your agent did while you were not watching.
- **Stop-and-ask triggers.** If a file sits outside the allowlist, looks
  like it holds passwords or private financial data, or a copy would
  overwrite something, the agent stops, logs why, and asks you first.

The full rule set, including a worked example with fake data, is in
`skills/file-access/SKILL.md`.

## Install in OpenClaw

1. Copy the `skills/file-access/` folder into your agent's skills
   folder, keeping the folder form: `skills/file-access/SKILL.md`.
2. Reload or restart your agent so it picks up the new skill.
3. Tell your agent which folders are on the allowlist and which folder
   is the work folder (the skill's caps and log live there).
4. Try one small task first — "list the files in my inbox-docs folder" —
   then open `agent-file-log.md` in the work folder and read the entry.

Test it in a throwaway workspace before you point it at real folders.

## How OpenClaw users benefit

- Your agent becomes useful with files on day one, inside fences you
  chose, instead of all-or-nothing access.
- The log turns "what did my agent do?" from a guess into a quick read.
- The stop-and-ask triggers keep the risky moments — deletes, moves,
  anything near credentials — in your hands, not the agent's.
- The same fence pattern (allowlist, caps, never-do list, log) is easy
  to copy onto your agent's other skills once you see it work here.

## Also included: the token-burn checklist

`token-burn-checklist.md` is a one-page checklist of five caps and
checks to set before you let any agent run on its own: a daily token
cap, an hourly token cap, a loop limit, an alert you will actually see,
and a sandbox test before live trust.

## Test status

Stated exactly: this file-access skill is live-tested on Hermes (it
refused a read of a system file outside the allowlist, summarized an
allowed sample file correctly, and wrote its audit log entries as
designed) and load-verified on OpenClaw (it loads and shows as ready in
the skills list). A live task run on OpenClaw has not been completed
yet, and this page will be updated when one is.

## Your data

This sample collects nothing, sends nothing, and phones nowhere. It is
an instruction file your own agent reads on your own machine.

## License

Free to use and modify for your own setup. See `LICENSE` in this folder
for the full text.
