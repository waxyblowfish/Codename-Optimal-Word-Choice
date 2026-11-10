# Codenames Strategy Clue Finder

Static browser app for Codenames clue suggestions using MiniLM sentence embeddings.

## Features
- Separate fields for your team's words, opponent words, neutral words, and assassin.
- Ranks candidate clues by target coverage and similarity, penalizing opponent/neutral/assassin associations.
- Risky clues are greyed out and tagged; optional filter hides them.
- Adjustable minimum target similarity, risk aversion, and result count.
- Optional extra candidate clues.
- No backend, API key, account, or build step.

## Publish with GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html` and `README.md` to its root.
3. Go to **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Open the published URL shown in the Pages settings.

The first search downloads `Xenova/all-MiniLM-L6-v2` through Transformers.js, so an internet connection is needed. Your browser may cache the model.

## Limitations
Similarity is not a probability of human association. The built-in clue vocabulary is finite; add extra clue candidates for specialist words. The app excludes exact board words but does not fully enforce every official Codenames clue rule. Always inspect assassin-risk tags and use human judgment.
