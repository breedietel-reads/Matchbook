# MatchBook: Developer Brief

**Launch target:** January 1, 2027. **Goal:** inspire people to read more, meet in real life, and explore their own city in the new year.

**What it is:** Readers log books they finish, tagged with their city. Once 5 readers in the same city log the same book, that city's message board opens (for example, "Where the Crawdads Sing: Atlanta"). A room holds up to 20 readers. After that, the next reader who logs it in that city is placed in a new room for the same book and city, which opens once 5 readers have joined it. Room numbers are internal and never shown to readers. Later, partner bars, restaurants and libraries host the club. We value real-life, safe, in-person experiences.

**Reference prototype:** https://claude.ai/artifact/NX8WurDtwTVoKHfpfX9TtW (clickable; data is stored only in the browser, so every feature below needs a real backend).

## Launch plan

- **Atlanta first.** Los Angeles and Philadelphia next. The city list should be easy to extend.
- **Platform:** a mobile-first responsive website, built as an installable web app. Native iPhone and Android apps come later, after launch.

## Version 1 features

**Accounts**
- Sign up with email, username (3 to 24 characters, unique, encouraged to use a favorite book, author, genre or character) and a password. Passwords are stored hashed.
- Email verification by 6-digit code before the account exists. One account per verified email.
- Profile: 25 preset profile pictures (our own art to be supplied), change city, change username, bookshelf of at most 8 books to discuss, and a "Past Book Clubs" list (book, author, "Discussed with" other readers).

**Books and logging**
- Readers pick from a verified catalog (Open Library or Google Books API). Each book has one canonical ID, so spelling variants cannot split the reader count. Include a "request a missing book" option.
- Unlimited logs per account, but only one log per book per account. Each log is stamped with the reader's city, and a "travelling" option lets them log in another city.
- A running log shows who read what and in which cities.

**Message boards**
- Rooms are per book and per city. A board opens when 5 readers in the same city have logged the same book. Progress shows as 5 layered cartoon flames (outlined until filled), blue and green, that all turn red and orange when the board opens. The flame artwork should follow the reference illustration set the founder supplied. Each room holds at most 20 readers; the 21st reader in that city is placed in a new room. Readers only ever see the book and city name (for example, "Where the Crawdads Sing: Atlanta") and their own progress toward 5, never a room number.
- Before posting, each reader answers one prompt (40 character maximum). Each new board gets one of five prompts at random, never the same as the previous board's: what made you pick up the book, what makes the author unique, a moment that stood out, which character stayed with you, what surprised you most. Answers appear as "Readers' first takes."
- Every board starts with a safety notice, then a separate quote message. Messages expire after 7 days of inactivity.

**Safety and moderation**
- A "Report this message" button on every message from another reader.
- Moderator queue (moderator logins only): remove message, remove and suspend user, or dismiss. Suspended users cannot post.
- Share buttons for the site on Threads, Instagram and TikTok, shown as icon buttons. The prototype uses generic placeholder icons; the real build should use each platform's official logo assets and follow its brand guidelines. Users do not share their own social accounts.

## Public website pages

Landing page, how it works, a "partner with us" form for bars, restaurants and libraries, community and safety guidelines, privacy policy, and terms of service.

## Look and feel

Colors: green #6bbd93, cream #fff2da, blue #3b78b0, plus orange #f26b21 and red #d62828 for the flames when a room opens. Light and dark modes. In dark mode, a very faint (about 5% opacity) upright handwriting pattern sits over the dark blue background. Wordmark in bold italic Playfair Display; headings in Fraunces. Generated book covers use a brand color with title and author in varied fonts (no uploads). The header shows the city, state abbreviation and a small state outline.

## Not in version 1

Native apps, direct messages, cover uploads, reading-verification quizzes, venue booking tools.

## Open decisions

1. **Small cities:** because rooms are per city, a book needs 5 readers in one city before it opens. Consider showing readers how many others in their city are waiting, and a way to be notified when a room opens.
2. **Who moderates**, and how fast must reports be answered? Boards lead to real meetups, so this needs a named person at launch.
3. **Age minimum** (suggest 18+) and legal review of the privacy policy and terms.
4. **The board quote:** using the full Naomi Shihab Nye passage needs the publisher's permission. The prototype uses only the first sentence.
5. **Portland:** the prototype assumes Oregon. Decide whether Portland, Maine is needed.
6. **Timeline:** about 12 weeks remain. Venue partnerships can start by hand after launch, so they are not needed on day one.
