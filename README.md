# SOS 110 — Live Class Game Demos

Two of the live classroom games from the SOS 110 slide decks, each wrapped in a
single page that plays itself.

Both games are normally played by a whole lecture hall at once, with every
student on their own phone and the instructor driving the phases from a
projected copy of the deck. That makes them almost impossible to show to one
person. So each game has a **self-running demo**: open it and a full class
joins, plays and finishes in a minute or two on the one screen, with a caption
strip explaining each beat.

Nothing is faked. The simulated students' choices go through exactly the same
model the real game uses, so the result is whatever that model actually
produces — including the runs where it does not go well.

| | |
|---|---|
| **[Tragedy of the Commons](commons/)** | 25 fishers, one lake, four rounds. Every student secretly chooses a harvest; the class total decides whether everyone sells at full price, everyone's payout falls, or the round pays nothing. |
| **[Evolve: Build an Organism](evolve/)** | 29 populations, one random world, ten generations. Everyone founds a population of 26 before anyone knows what the world looks like; then a barrier splits the class in two and the halves are compared, species by species. |

These pages never connect to a live class session: the whole game runs in the
browser that opened it.

## Rebuilding

Both pages are generated from the same deck engine that builds the lecture
decks, so a change to either game reaches the demos on the next build.

```
cd _deck-builder
python3 demo_site.py      # rebuild the pages
python3 shots.py          # re-capture the cover images (headless Chrome)
```
