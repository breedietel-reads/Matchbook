# Build MatchBook yourself with Claude Code

## Before you start
- You need a paid Claude plan (Pro or Max). The free plan does not include Claude Code.
- You need a Mac, Windows, or Linux computer. On Windows you may also need Git for Windows or WSL.
- GitHub is optional. It is a free place to back up your code. You can add it later.
- Expect a few hours a week. Today is mid-October, so you have about 11 weeks before January 1. Launching in Atlanta only, with a smaller first version, is realistic.

## Step 1: Install
Easiest: open the Claude desktop app and use its Code tab, so you don't need a terminal. Or install it in a terminal:
- Mac or Linux: `curl -fsSL https://claude.ai/install.sh | bash`
- Windows (PowerShell): `irm https://claude.ai/install.ps1 | iex`

Then sign in with your Claude account when it asks. Official instructions: https://code.claude.com/docs/en/getting-started/installation

## Step 2: Make your project folder
1. Create a folder called `matchbook`.
2. Put these four files in it: `CLAUDE.md`, `BUILD-GUIDE.md`, `matchbook-demo.html`, and the developer brief renamed to `matchbook-brief.md`.
3. Open Claude Code inside that folder. It reads `CLAUDE.md` automatically.

## Step 3: Build in phases
Paste each prompt, let it finish, test it, then move on.

1. **Plan.** "Read CLAUDE.md, matchbook-brief.md and matchbook-demo.html. Propose a simple setup for hosting, accounts and the database that I can own and run for free at small scale. Explain the trade-offs in plain language. Do not build anything yet."
2. **Website shell.** "Build the public pages and the app screens to match the demo's look. No real data yet."
3. **Accounts.** "Add sign-up with email verification, usernames, and city selection."
4. **Logging and rooms.** "Add the book search, logging, per-city rooms, the 20-reader limit, and the flame counters."
5. **Boards.** "Add the prompt before joining, the message board, the safety notice, and 7-day expiry."
6. **Safety tools.** "Add message reporting and the moderator page."
7. **Review.** "Review the whole project for security and privacy problems and fix them. Then write the test checklist I should run."

## Step 4: Save your work
Ask: "Set up Git so my work is saved with history." Optionally, create a free private GitHub repository and ask Claude Code to connect it for backup. Keep it private.

## Step 5: Test with friends, then a small launch
Test with a few friends first, then open to a small group in Atlanta. Keep your domain name registered in your own name.

## Before strangers use it
Meetups with strangers raise the stakes, so do these first:
- Privacy policy and terms of service, reviewed by someone qualified.
- An age minimum (suggest 18+).
- A named moderator who checks reports every day.
- A security check by someone technical, if you can find one. A single hour of a freelancer's time costs far less than a full build.

## When you get stuck
Tell Claude Code: "Explain what just happened in plain language and what my options are." Keep NOTES.md updated so you can pick up where you left off.
