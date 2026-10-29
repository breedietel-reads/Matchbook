# MatchBook: instructions for Claude Code

## About the owner
The owner is not a programmer. Explain things in plain language, work in small steps, and say what you are about to do before you do it. Ask before any decision that costs money, changes what users see, or is hard to undo. Never add features that are not in the brief.

## What we are building
MatchBook is a website where readers log books they finish, tagged with their city. Read `matchbook-brief.md` for the full requirements and `matchbook-demo.html` for the look and feel (open it in a browser). The demo is a click-through only; copy its design, wording, colors, and flame counters.

## Rules that must never be broken
- Rooms are per book and per city. A message board opens when 5 readers in the same city have logged the same book. A room holds 20 readers; the next reader goes into a new room. Room numbers are never shown to users.
- Before posting, each reader answers one short prompt (40 characters maximum).
- Every board starts with the safety notice from the demo. Messages expire after 7 days of inactivity.
- Email verification is required. One account per email, and one log per book per account.
- Reporting and moderator tools are part of version 1, not an extra.
- Users never share their own social media accounts in the app.

## Security
- Never write passwords, API keys, or secrets into the code. Use environment variables and tell the owner what to set.
- Use a trusted sign-in service for accounts and passwords instead of writing our own.
- Restrict database access so users can only change their own data.
- Collect as little personal information as possible.

## How to work
- Build in the phases listed in `BUILD-GUIDE.md`. Finish and test one phase before starting the next.
- Save progress with Git often, with clear messages.
- Before saying something works, run it and test it. Tell the owner how to check it too.
- Keep a short `NOTES.md` listing what exists, what is left, and any settings the owner must configure.
