<img align="right" alt="GIF" width="172" height="258" src="https://github.com/user-attachments/assets/23135f6f-6cc4-4324-97bb-4dc56fe3d347" />

# Hello world!

I like building things that can back up their own results: machine-learning
and language-model experiments that anyone can rerun and check, and apps with
tests on the parts that are hard to get right. Mostly Python and TypeScript,
some Java.

**[LinkedIn](https://www.linkedin.com/in/qkennethkimbrough/)**

## Featured projects

### [Renart](https://github.com/kennethkimbrough/Renart) — which Renaissance master painted it?

Ranks which of ten painters made a painting from its style alone. A fine-tuned
ResNet-18 gets **77.7% right** (96% with the painter in its top 3) against
52.6% for a classical baseline, and an independent rerun reproduced every
number exactly.

**[Results site](https://kennethkimbrough.github.io/Renart/)** · *Python · PyTorch · scikit-learn · GitHub Actions*

### [tit-for-token](https://github.com/kennethkimbrough/tit-for-token) — how language models play repeated games

Tournaments of the iterated prisoner's dilemma between language models from
four labs and classic strategies like Tit-for-Tat, recorded so every match
replays byte-for-byte. In the first 400 matches, Claude Haiku and DeepSeek
played almost exactly like Grim Trigger, while Gemini Flash cooperated far
less (49% of its rounds against Haiku's 81%).

**[Results site](https://kennethkimbrough.github.io/tit-for-token/)** · *Python (standard library only) · asyncio · bootstrap statistics · GitHub Actions*

### [Outage Ready](https://github.com/kennethkimbrough/outage-ready) — how long your household lasts in an outage

A simulator rather than a checklist: enter what you have and how your home
works, and it plays each outage forward hour by hour to show how long you are
covered, what fails first and what to do now. Installs as an app, works fully
offline and keeps all data on the device.

**[Live app](https://kennethkimbrough.github.io/outage-ready/)** · *TypeScript · no framework · service worker · Playwright end-to-end tests*

### Biscuit's Bowls — a cat-café logic-puzzle game

A 100-puzzle campaign with Endless, Rush Hour, and co-op and versus
multiplayer, heading for an iPhone release (source private). Two phones stay
in sync over plain HTTP and one SQLite database, with the server checking
every move and database constraints settling the races.

**[How the multiplayer works](https://github.com/kennethkimbrough/kennethkimbrough/blob/main/biscuits-bowls-multiplayer.md)** · *TypeScript · React / Next.js · Cloudflare Workers · Drizzle ORM*

## Elsewhere

- [mlb-injuries](https://github.com/kennethkimbrough/mlb-injuries) — Java tracker for MLB's injured lists: a daily snapshot from the public MLB Stats API and reports on who has been out longest. Maven, JUnit 5.
- [trending-songs-finder](https://github.com/kennethkimbrough/trending-songs-finder) — Python tracker for Spotify's new releases that reports what entered, dropped off and stayed longest. MySQL, Docker.
