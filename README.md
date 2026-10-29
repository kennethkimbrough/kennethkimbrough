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

## Elsewhere

- [trending-songs-finder](https://github.com/kennethkimbrough/trending-songs-finder) — small Python service that pulls track recommendations from the Spotify API into MySQL, with unit tests and a Dockerfile.
- [mlb-injuries](https://github.com/kennethkimbrough/mlb-injuries) — Java client that lists currently injured MLB players from the SportsData.io API.
