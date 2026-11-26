# wordly

A clean, editorial vocabulary hub. One homepage, five study lists. Pick a list, flip the cards, take the quiz — progress is saved in your browser.

**Live site:** https://donquixote-doflaming.github.io/wordly/

---

## Lists

| Card | File | Words |
|---|---|---|
| GRE Vocab | `gre-vocab.html` | 1,111 |
| Vocab 400 | `vocab-400.html` | 400 |
| Vocab 520 | `vocab-520.html` | 520 |
| A-Z Vocab | `vocab-a-z.html` | 1,925 |
| Word Smart I (Bangla) | `word-smart-i.html` | 830 |

## Features

- White editorial UI with an electric-blue accent (`#00f`), hand-drawn blue scribble marks, and handwriting notes (Caveat)
- Work Sans display type, Open Sans body text, system mono for labels
- Five list cards on the homepage with live per-list progress bars
- Flashcards with 3D flip: meaning, pronunciation, synonyms, antonyms, example
- Quiz modes: synonym, antonym, Bangla, fill in the blank
- Mastered words are tracked per list in `localStorage` and reflected on the homepage
- Keyboard controls on flashcard decks (`←` again, `→` next, `Space` flip, `M` mastered, `Esc` groups)
- Responsive layout with `prefers-reduced-motion` support
- Pure HTML and CSS, no build step, no dependencies

## Project structure

```
CYBER-VOCAB/
├── index.html
├── brain.png                    (favicon)
├── gre-vocab.html
├── vocab-400.html
├── vocab-520.html
├── vocab-a-z.html
├── word-smart-i.html
└── README.md
```

All links are relative, so `index.html` and the five list pages must stay in the same folder.

## Run locally

1. Clone or download the repository.
2. Open `index.html` in any modern browser.



## Deploy on GitHub Pages

1. Push all files to the repository root.
2. Go to **Settings → Pages**.
3. Under **Source**, choose the `main` branch and the `/ (root)` folder, then save.
4. The site goes live at https://rifat440.github.io/CYBER-VOCAB/

## Fonts

Work Sans, Open Sans, and Caveat are loaded from Google Fonts. Bangla text uses Tiro Bangla. Without an internet connection the page falls back to system fonts and everything else still works.

## Customize

- **Accent color:** the `--blue` custom property in each page's `<style>` block (`#00f` by default).
- **Card text and links:** edit the five `<a class="card">` blocks in `index.html`.
- **Progress keys:** each card's `data-key` / `data-total` must match the localStorage key and word count of its list page.

---

*Prepared by Rifat · Revision data stays in this browser · No accounts, no tracking*
