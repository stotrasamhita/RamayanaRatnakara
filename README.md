# रामायण-रत्नाकरः · Rāmāyaṇa Ratnākara

A LaTeX/Devanāgarī collection of Rāma-kathā — retellings, episodes, and stotras connected to
the Rāmāyaṇa — gathered from across the Itihāsas and Purāṇas, not just the Vālmīki Rāmāyaṇa
itself. Part of the [StotraSamhita](https://github.com/stotrasamhita) family of Sanskrit-text
projects.

## What's here

The compiled book (`ramayana-ratnakara-mulam.tex`/`.pdf`) assembles four parts, each drawn from its own folder:

| Part (as titled in the book) | Folder | Contents |
|---|---|---|
| राम-चरितानि (Rāma-caritāni) | [`rama-charitam/`](rama-charitam/README.md) | Retellings/summaries of Rāma's story as they occur *within* other texts — 19 different Itihāsas/Purāṇas, including the Vālmīki Rāmāyaṇa's own internal condensations (*Saṅkṣepa Rāmāyaṇam*, *Gāyatrī Rāmāyaṇam*, etc.). |
| रामायणान्तर्गताः कथाः (stories within the Rāmāyaṇa) | [`katha/`](katha/README.md) | Side-stories and episodes embedded in the Rāmāyaṇa narrative, drawn from 8 different Purāṇas. |
| रामायणान्तर्गत-स्तोत्राणि (Rāmāyaṇa-related stotras) | [`stotram/`](stotram/README.md) | *Nāma-rāmāyaṇam* and two other stotras connected to the Rāma story. |
| अनुबन्धाः (appendices) | [`anubandha/`](anubandha/README.md) | Dhyāna/maṅgala verses, the Rāmāyaṇa-māhātmyam from the Skanda Purāṇa, and a Nāmāvali section — the last of these pulls its content from the **sibling `namavali-manjari` repository** (see [Building](#building) below). |

Also at the root:

- `ramayana-ratnakara-mulam.tex` / [📄 `.pdf`](https://github.com/stotrasamhita/ramayanaratnakara/blob/main/ramayana-ratnakara-mulam.pdf) — the compiled book, `\input`-ing all four parts above in order.
- `frontmatter/` — title page (`cover-mulam.tex`), Sanskrit preface (`preface-mulam.tex`, see below), and shared LaTeX preamble (`preamble-mulam.tex`).
- `shloka.sty` — the custom style package with the verse-typesetting macros used throughout.
- [`source/`](source/README.md) — raw/working source text (OCR output, chapter-split drafts) for a few of the Purāṇas, kept for reference; not `\input` by the book.
- [`stories/`](stories/README.md) — a planned English-language companion (translations/summaries), currently just a scaffold with no content yet.

## Building

The document is written for **XeLaTeX** (see the `% !TeX program = XeLaTeX` line in `ramayana-ratnakara-mulam.tex`), using `fontspec` with the **Adobe Devanagari** font. You'll need a TeX distribution with XeLaTeX (e.g. TeX Live).

**Cross-repo dependency:** the appendices' Nāmāvali section `\input`s files directly from `../namavali-manjari/100/*.tex` (see `anubandha/README.md`). To build the full book, clone [`namavali-manjari`](https://github.com/stotrasamhita/namavali-manjari) as a **sibling directory** of this repo (i.e. both under the same parent folder) before running XeLaTeX.

```sh
xelatex ramayana-ratnakara-mulam.tex
xelatex ramayana-ratnakara-mulam.tex   # run twice for the table of contents
```

There is currently only one compiled edition — no separate Kindle/print variants have been produced yet (the `.tex` file has `kindle`/`print` `etoolbox` booleans wired up for this, both currently set `false`).

## The preface

`frontmatter/preface-mulam.tex` (in Sanskrit) opens by observing that listeners of the Rāmāyaṇa never tire of it — quoting Vālmīki's own line that people's talk became "Rāma, Rāma, Rāma" (*rāmo rāmo rāma iti*), and Sītā's remark in the Adhyātma Rāmāyaṇa, during the exile in the forest, that she has "heard the Rāmāyaṇa recited many times, by many *dvijas*." It explains the book's purpose: to gather in one place the many Rāma-stories scattered across the Itihāsas and Purāṇas — some closely following Vālmīki, some going beyond it into stranger episodes found only in certain other texts (e.g. a Padma Purāṇa passage where Rāma himself questions Mahādeva), and some expanding at length on episodes only briefly touched in Vālmīki's own text. It notes that even within the Mahābhārata, Bhīṣma, Hanumān (to Bhīma), and Nārada each narrate Rāma's story in different contexts — especially Mārkaṇḍeya's extensive telling in the *Rāmopākhyāna Parva* of the Vana Parva. It closes with salutations to Vyāsa and Vālmīki as the tellers of these stories, and a prayer for unwavering devotion to Rāma. It is dated Āṣāḍha-Kṛṣṇa-Dvādaśī (Viśvāvasu saṃvatsara), July 22, 2025, and signed at *Sarvajñātma-Pratiṣṭhānam*.

## Acknowledgements

From the colophon: gratitude to the volunteers who scanned old texts, performed OCR, and uploaded them to Wikisource and other repositories — this collection is a compilation drawing on that work — and to [wisdomlib.org](https://www.wisdomlib.org) for indices and translations of the Purāṇas that made searching them easier. The preface explicitly frames the project as an early, "version 0.1" milestone rather than a finished, fully proofread edition — more a start worth publishing than a completed critical text.

## Usage

No separate LICENSE file is included in this repository. See the [StotraSamhita](https://github.com/stotrasamhita) organization for related projects and [stotrasamhita.net](https://stotrasamhita.net).

## 📑 Index

**Jump to:** [What's here](#whats-here) · [Building](#building) · [The preface](#the-preface) · [Acknowledgements](#acknowledgements) · [Usage](#usage)

**All release PDFs:**

| Edition | PDF |
|---|---|
| Complete book | [📄 ramayana-ratnakara-mulam.pdf](https://github.com/stotrasamhita/ramayanaratnakara/blob/main/ramayana-ratnakara-mulam.pdf) |

**Read it online, in multiple scripts:** not yet published — [stotrasamhita.github.io](https://github.com/stotrasamhita/stotrasamhita.github.io) currently has no section for this repo (its "Adhyatma Ramayanam" section is sourced from a separate, dedicated `adhyatmaramayanam` repo, not from here).

---

*The README.md files on this repo were generated and beautified with Claude.*
