# Codenames Strategy Clue Finder

Static browser app for Codenames clue suggestions using MiniLM sentence embeddings.

## Features
- Separate fields for your team's words, opponent words, neutral words, and assassin.
- Ranks candidate clues by target coverage and similarity, penalizing opponent/neutral/assassin associations.
- Risky clues are greyed out and tagged.
- Adjustable minimum target similarity, risk aversion, and result count.
- Optional extra candidate clues.
- No backend, API key, account, or build step.

The first search downloads `Xenova/all-MiniLM-L6-v2` through Transformers.js, so an internet connection is needed. Your browser may cache the model.

## Limitations
Similarity is not a probability of human association. The built-in clue vocabulary is finite; add extra clue candidates for specialist words. The app excludes exact board words but does not fully enforce every official Codenames clue rule.
