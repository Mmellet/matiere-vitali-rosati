# C'est la matière qui pense

Repos du livre _C'est la matière qui pense_, leçon inaugurale de la Chaire d'excellence en édition numérique de Marcello Vitali-Rosati, prononcée le 23 octobre 2024.

Ce livre est le premier volume de la collection Arion aux Presses de l'Université de Rouen et du Havre et fait l'objet d'ue double publication numérique et papier.

## Produire le livre

Le livre est écrit en markdown. Le fichier du texte est [texte.md](texte.md).

Le pdf est créé grâce au fichier [livre.tex](livre.tex) qui  défini le template et inclut le texte en tex transformé par pandoc.

La transformation se fait avec un make:

- `make fab` production du livre
- `make serve` production du livre en temps réel à chaque fois qu'il y a une modification avec `entr`

Le pdf est créé en utilisant `luaLaTeX`. On utilise le paquet minted pour le code.

## Dépendances

- `texlive-full`
- `pandoc`
- `entr`


