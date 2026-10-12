# NeuroDual — word game data (2026-10-12)

Word lists and crossword clues used by the language games of NeuroDual
(Word or Not, Mystery Word, Word Ladder, Letter Grid, Crossword).

These files are adaptations of the sources listed in `word-lists/CREDITS.md`
and `crossword-clues/CREDITS.md` (Wiktionary, FrequencyWords, Lexique,
wordfreq, LDNOOBW, ENABLE2K). They are licensed under the **Creative Commons
Attribution-ShareAlike 4.0 International** licence (CC BY-SA 4.0):
<https://creativecommons.org/licenses/by-sa/4.0/>. You may copy, modify and share them, including
commercially, provided you give credit and share your adaptations under the
same licence. The licence covers these data files only, not the NeuroDual
application.

They are provided as is, without warranty of any kind (sections 5 and 6 of
the licence).

## Contents

- `word-lists/<lang>.txt` — the lists exactly as the application reads them
  (format 2: prefix-coded trie, header lines start with `#`). Languages:
  cs, da, de, el, en, es, fi, fr, it, nl, no, pl, pt, ro, ru, sv, uk.
- `word-lists-tsv/<lang>.tsv` — the same lists decoded, one accepted word form
  per line: `word` (spelling shown to players), `key` (folded comparison
  key), `band` (frequency rank: 0 ≤ 1,000, 1 ≤ 3,000, 2 ≤ 10,000,
  3 ≤ 30,000, 4 attested beyond, 5 unknown), `flags` (P proposable,
  L dictionary headword, Q offensive — accepted but never shown, R rare).
- `crossword-clues/<lang>.txt` — one headword per line followed by one or
  two definitions, tab-separated. Languages: en, fr.

## Changes made to the sources

See the "Modifications" paragraphs of both `CREDITS.md` files: selection of
word forms (part of speech, length, script), removal of proper nouns,
acronyms, abbreviations and phrases, marking of offensive and rare words,
folding into comparison keys, frequency bands, prefix coding; for clues,
selection of at most two definitions, removal of cross-references and of
definitions that reveal the answer, shortening of long definitions.

---

# NeuroDual — données des jeux de langue

Listes de mots et indices de mots croisés des jeux de langue de NeuroDual,
adaptés des sources citées dans les deux `CREDITS.md` et distribués sous
licence CC BY-SA 4.0 (<https://creativecommons.org/licenses/by-sa/4.0/>), sans garantie. Vous pouvez les
copier, les modifier et les partager, y compris commercialement, en citant
les auteurs et en partageant vos adaptations sous la même licence.
