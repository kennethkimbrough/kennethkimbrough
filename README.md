<img align="right" alt="GIF" width="172" height="258" src="https://github.com/user-attachments/assets/23135f6f-6cc4-4324-97bb-4dc56fe3d347" />

# Hello world!

I build backend and data projects in Java, Python and JavaScript/TypeScript,
and I'm always up for collaborating on open-source work.

## Featured projects

### [Renart](https://github.com/kennethkimbrough/Renart) — style-based artist attribution for Renaissance paintings

Given a photograph of a Renaissance painting, Renart ranks which of ten
painters most likely made it, from style alone. It is a reproducible
pipeline: the data download, a classical baseline (102 hand-crafted colour
and brush-stroke features into a logistic regression) and a fine-tuned
ResNet-18 all run from one GitHub Actions workflow, and every reported number
comes from a committed run.

Latest run (1,653 WikiArt images, 327 held out for validation, 13 minutes of
training on a CPU runner): the CNN reaches **77.7% accuracy and 96.0% top-3
accuracy**, against 52.6% for the classical baseline and 10% chance. The
confusions are the ones an art historian would predict, such as the three
Venetians (Titian, Tintoretto, Veronese) with each other, and Grad-CAM
heatmaps show where the network looks. It is not an authentication tool:
style cannot separate a master from a good copy.

*Python · PyTorch · scikit-learn · GitHub Actions*

### [tit-for-token](https://github.com/kennethkimbrough/tit-for-token) — how language models play repeated strategic games

Round-robin tournaments of the iterated prisoner's dilemma between language
models from different labs and classic strategies like Tit-for-Tat. Every
model call is recorded, so a tournament replays byte-for-byte without the
network, and CI re-checks the committed results on every push. The report
measures cooperation, retaliation, forgiveness and exploitation, each with a
bootstrap confidence interval.

First tournament (400 matches): Claude Haiku and DeepSeek Flash played almost
exactly like Grim Trigger, cooperating until betrayed and then almost never
forgiving, while Gemini Flash cooperated in 49% of its rounds against
Haiku's 81%. A dry run caught reasoning models being cut off mid-thought and
recorded as defecting; the report now marks a player's results invalid
whenever that happens often enough to distort them.

*Python (standard library only) · asyncio · record and replay · bootstrap statistics · GitHub Actions*

### [Outage Ready](https://github.com/kennethkimbrough/outage-ready) — what your household can sustain in an outage

**Live:** https://kennethkimbrough.github.io/outage-ready/

Most preparedness advice is a checklist; Outage Ready is a simulator. You
enter what you have on hand and how your home works (pumped or gravity water,
electric or gas cooking, fridge and freezer), and it plays each outage
scenario forward hour by hour, following the dependencies in your home, to
tell you how long you are covered, what fails first and why, and what to do
now. It installs as a PWA on desktop and mobile, works fully offline after the
first visit, and keeps all data on the device.

*TypeScript · plain ES modules, no framework or bundler · service worker ·
Playwright end-to-end tests*

### Biscuit's Bowls — a cat-café logic-puzzle game

**Play it:** https://cat-cafe-v50-test.epicsigmaker.chatgpt.site

Place food bowls so every cat has exactly one neighbouring bowl. A 100-puzzle
campaign across four chapters, 17 bonus tables, Endless and Rush Hour modes,
and co-op and timed-versus multiplayer, plus a café of 21 collectable cats to
look after between puzzles. Accounts, cloud saves and multiplayer run on
Cloudflare Workers with a database behind them; the puzzles themselves work
offline. The source is private ahead of an iPhone release.

*TypeScript · React / Next.js · Cloudflare Workers · Drizzle ORM · screenshot-based release checks*

## Elsewhere

- [mlb-injuries](https://github.com/kennethkimbrough/mlb-injuries) — Java command-line tracker that reads MLB's injured lists from the public MLB Stats API, records a daily snapshot, and reports who has been out longest and which teams are hit hardest. Maven, JUnit 5, scheduled GitHub Actions run.
- [trending-songs-finder](https://github.com/kennethkimbrough/trending-songs-finder) — Python tool that stores Spotify's new-releases list in MySQL on each run and reports what entered, dropped off, moved, and stayed longest. Unit tests, Docker.
