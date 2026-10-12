# Crédits et licence des indices des mots croisés

Les fichiers `<lang>.txt` de ce dossier (en, fr) sont des œuvres dérivées,
distribuées sous **Creative Commons Attribution-ShareAlike 4.0 International
(CC BY-SA 4.0)** <https://creativecommons.org/licenses/by-sa/4.0/>.

Ils ne sont pas à éditer à la main : `scripts/crossword/build-crossword-clues.ts`
les construit. Modifications apportées aux sources : sélection des mots que le
jeu peut placer (mots-vedettes à proposer des lexiques du dossier
`../word-lists/`, même graphie), choix d'au plus deux définitions parmi les
trois premiers sens, écarts des renvois, des définitions qui contiennent la
réponse ou sa racine, des prénoms et lieux, des sens rares, régionaux ou
grossiers, coupe des définitions longues, liste d'exclusion relue
(`scripts/crossword/clue-exclusions.ts`).

La licence ne porte que sur ces fichiers, pas sur le code de l'application.
Ils sont fournis tels quels, sans garantie d'aucune sorte (sections 5 et 6 de
la licence).

## Sources

- **Wiktionnaire** (édition française de Wiktionary), contributeurs du
  Wiktionnaire, <https://fr.wiktionary.org/>, extrait par **wiktextract**
  (Tatu Ylonen), <https://kaikki.org/frwiktionary/> (édition du 2026-09-22).
  Licences CC BY-SA 4.0 et GFDL ; utilisé ici sous CC BY-SA 4.0. → `fr.txt`
- **Wiktionary** (édition anglaise), contributeurs de Wiktionary,
  <https://en.wiktionary.org/>, extrait par **wiktextract** (Tatu Ylonen),
  <https://kaikki.org/dictionary/> (édition du 2026-09-20). Licences
  CC BY-SA 4.0 et GFDL ; utilisé ici sous CC BY-SA 4.0. → `en.txt`

  Ylonen, T. (2022). Wiktextract: Wiktionary as Machine-Readable Structured
  Data. *Proceedings of LREC 2022*.
- **List of Dirty, Naughty, Obscene, and Otherwise Bad Words** (LDNOOBW),
  © 2012–2020 Shutterstock, Inc. et contributeurs, CC BY 4.0 : sert à
  écarter les définitions qui citent un mot grossier.

## Obligations

Comme les lexiques (`../word-lists/CREDITS.md`, section « Obligations ») :
mentions de l'application (`THIRD_PARTY_NOTICES.txt`, Paramètres › À propos ›
Licences et crédits), aucune restriction ajoutée, et copie publique dans le
même paquet que les listes (`scripts/word-lists/package-open-data.ts`).
