# Crédits et licence des lexiques

Les fichiers `<lang>.txt` de ce dossier (cs, da, de, el, en, es, fi, fr, it,
nl, no, pl, pt, ro, ru, sv, uk) sont des œuvres dérivées, distribuées sous
**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**
<https://creativecommons.org/licenses/by-sa/4.0/>.

Modifications apportées aux sources : sélection des formes (catégorie
grammaticale, longueur de 2 à 15 graphèmes, écriture de la langue), retrait
des noms propres (étiquette de Wiktionary et casse dans Tatoeba), sigles,
abréviations, interjections et locutions, marquage des mots
grossiers et rares, repli en clé de comparaison, calcul d'une bande de
fréquence, codage par préfixe. Voir `scripts/word-lists/` (chaîne de
construction) et `packages/logic/src/domain/words/lexicon.ts` (format).

La licence ne porte que sur les listes, pas sur le code de l'application. Les
listes sont fournies telles quelles, sans garantie d'aucune sorte (sections 5
et 6 de la licence).

## Sources communes

- **Wiktionary**, édition anglaise, contributeurs de Wiktionary,
  <https://en.wiktionary.org/>, extrait par **wiktextract** (Tatu Ylonen),
  <https://kaikki.org/> (édition du 2026-09-20). Licences CC BY-SA 4.0 et
  GFDL ; utilisé ici sous CC BY-SA 4.0.
  Ylonen, T. (2022). Wiktextract: Wiktionary as Machine-Readable Structured
  Data. *Proceedings of LREC 2022*.
- **FrequencyWords**, Hermit Dave, <https://github.com/hermitdave/FrequencyWords>
  (révision 525f9b5), listes 2018 tirées des sous-titres d'OpenSubtitles
  (<http://www.opensubtitles.org/>, via OPUS). Contenu sous CC BY-SA 4.0.
  Rang de fréquence de cs, da, de, el, en, es, fi, it, nl, no, pl, pt, ro,
  ru, sv.
- **List of Dirty, Naughty, Obscene, and Otherwise Bad Words** (LDNOOBW),
  © 2012–2020 Shutterstock, Inc. et contributeurs,
  <https://github.com/LDNOOBW/List-of-Dirty-Naughty-Obscene-and-Otherwise-Bad-Words>
  (révision 5faf2ba). Licence CC BY 4.0
  <https://creativecommons.org/licenses/by/4.0/>. Utilisée pour marquer des mots,
  dans leur langue et dans les gloses anglaises de Wiktionary.

- **Tatoeba**, contributeurs de Tatoeba, <https://tatoeba.org/>, exports
  de phrases par langue (<https://downloads.tatoeba.org/exports/per_language/>,
  relevés le 2026-10-12). Licence CC BY 2.0 FR. Aucune phrase n'est livrée :
  la casse des formes au milieu des phrases sert seulement à écarter les noms
  propres des mots à proposer (toutes les langues livrées sauf l'allemand).

## Sources propres à une langue

- **Français** — **Lexique 3.83**, Boris New, Christophe Pallier et
  contributeurs, <http://www.lexique.org>,
  <https://github.com/chrplr/openlexicon>. Licence CC BY-SA 4.0. Formes et
  fréquences (livres et sous-titres).
  New, B., Pallier, C., Brysbaert, M., & Ferrand, L. (2004). Lexique 2: A New
  French Lexical Database. *Behavior Research Methods, Instruments, &
  Computers*, 36(3), 516–524.
- **Anglais** — **ENABLE2K** (Enhanced North American Benchmark LExicon),
  Alan Beale et M. Cooper, domaine public ; copie de
  <https://github.com/BartMassey/wordlists> (révision af52415).
- **Ukrainien** — **wordfreq**, Robyn Speer, <https://github.com/rspeer/wordfreq>
  (révision 912caf6), liste `large_uk`. Données sous CC BY-SA 4.0 ; pour
  l'ukrainien, elles sont tirées de Wikipédia, d'OpenSubtitles (via OPUS),
  de textes du web (OSCAR), de Twitter et de Reddit (tableau des sources et
  section « License » de son README).

## Construites, non livrées

La chaîne produit aussi des listes pour les 21 autres langues de l'app,
gardées hors du dépôt tant qu'elles ne sont pas retenues. Le swahili et le marathi y
prennent leurs fréquences d'un vidage daté de **Wikipédia** (2026-09-01,
CC BY-SA 4.0) ; à citer ici le jour où elles sont livrées.

## Obligations

- Garder ce fichier avec les listes. Les mentions de l'application
  (`apps/web/public/THIRD_PARTY_NOTICES.txt`, affichées dans Paramètres ›
  À propos › Licences et crédits) en reprennent l'essentiel : auteurs,
  licence et son adresse, absence de garantie, modifications. La garde
  `apps/web/src/data/word-game-licence.test.ts` vérifie que chaque source
  d'un en-tête `#sources` y est créditée.
- N'ajouter aucune restriction aux droits de la licence : les CGU et les
  mentions légales en exceptent les listes.
- Copie publique sous CC BY-SA 4.0, avec ce fichier : le paquet de
  `scripts/word-lists/package-open-data.ts`, déposé à l'adresse
  `WORD_GAME_DATA_PUBLICATION_URL` (`apps/web/src/data/word-game-licence.ts`).
  Tant que cette adresse est vide, aucun jeu de langue ne sort du retrait
  (même garde).
