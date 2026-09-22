# SOS 110 — Live Class Game Demos

Four of the live classroom games from the SOS 110 slide decks, each wrapped in
a page that plays itself.

The games are normally played by a whole lecture hall at once, with every
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
| **[Build a Nation](nation/)** | 29 nations, sixty years, two event cards, and a second try. Everyone spends 14 points on policy before learning where their nation starts; population pyramids reshape as the years run, event cards test each plan, and a revision shows what changing course does. |
| **[Module 1 &amp; 2 Review Game](review/)** | 25 students, ten questions, a Word Puzzle, Connections and a reflex break. This one shows two screens at once, the projector and a student's phone, because half the game happens in the student's hand. |

These pages never connect to a live class session: the whole game runs in the
browser that opened it.

## Rebuilding

Every page is generated from the same deck engine that builds the lecture decks,
so a change to any of these games reaches the demos on the next build. The
review demo also copies in the photos its picture questions use.

```
cd _deck-builder
python3 demo_site.py      # rebuild the pages
python3 shots.py          # re-capture the cover images (headless Chrome)
```
