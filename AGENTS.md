# AGENTS

Organization-wide rules for Head Up agents come from the handbook. This file adds only what is
specific to this repository.

## What this repository is

The legal texts of Head Up, in `texts/`: one HTML file per text and language. They are page sources
that the website builds into headup.me. The website and the API pin a tag of this repository.

## Rules

- Change a text only when the owner asks for that change. Never reword, reorder or improve a legal
  text on your own initiative.
- A change to what a text says needs a new version. In the same pull request, update every file
  whose version line states that version, in every language, and keep the languages saying the same
  thing. One identifier can appear in several texts: `privacy-minor-vN` is on the version line of
  both `texts/privacy*.html` and `texts/child-privacy*.html`.
- After the owner merges, create a signed tag for each version on a version line that has no tag yet,
  named exactly as the version, for example `privacy-v15`. Never move or delete a tag.
- Keep the placeholders listed in `README.md` as they are; the website fills them.
- Formatting must pass `npx --yes prettier@3.9.6 --check .`, which the Format workflow runs.
