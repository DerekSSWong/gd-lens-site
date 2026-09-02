# GD Lens

Drop a Grim Dawn save in and see the character behind it, published at
**https://dereksswong.github.io/gd-lens-site/**

- equipped gear with full rolled names, masteries, skills and devotion
- a character sheet where **every stat expands to the sources that produced it**
- a verdict on every row — priority, nice to have, ignore — that you can override
  by clicking it
- **a loot filter graded for your character**: every prefix and suffix in the game
  coloured by what it is worth to *this* build, as a Grim Raynbow `text_en`
  override you drop into `<Grim Dawn>/settings/text_en/`

The page opens on a **bundled sample character** so there is something to look at
straight away; drop your own `.gdc` on it to replace them.

## Your save never leaves your machine

There is no upload and no server. The page is one self-contained HTML file: it
decrypts the `.gdc`, sums the stats and grades the affixes **in your browser**.
Close the tab and nothing of yours remains anywhere but your own disk.

## This repo is output, not source

`index.html` is generated — **never hand-edit it**. It is built from the game's own
records by a separate private pipeline, which reads a local extraction of the game
database that cannot live in a repo, and it is only published after every gate
passes. An edit made here is lost on the next build.

## Credits

The loot filter is built on top of
[Grim Raynbow](https://forums.crateentertainment.com/) — its colour file is the
template the grades are written into.
