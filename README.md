# langage-clair-fr

Skill pour écrire en français des textes que des lecteurs non-experts comprennent **à la première lecture**, sans avoir à relire ni demander de l'aide.

Croise quatre référentiels :

- **FALC** : Facile à Lire et à Comprendre (Inclusion Europe, UNAPEI)
- **Langage Clair** : DITP / modernisation.gouv.fr
- **Plain Language** : tradition anglo-saxonne (PLAIN, plainlanguage.gov)
- **Flesch FR** : formule de lisibilité Kandel-Moles (1958)

## À qui ça s'adresse

Le skill est pensé pour les contextes où la clarté du texte est une **question d'équité d'accès**, pas un choix stylistique :

- Droit du travail, droits sociaux, démarches administratives
- Santé, éducation, services publics
- UI, emails transactionnels, FAQ pour grand public
- Vulgarisation de textes juridiques ou techniques

Il ne s'applique **pas** à la doc dev interne, au marketing à effet stylistique, ni à la poésie.

## Ce que le skill contient

- 10 règles non-négociables (une idée par phrase, voix active, verbes plutôt que noms, etc.)
- Un lexique de substitution **bureaucratique vers clair** (environ 25 entrées)
- Une liste d'anti-patterns FR fréquents
- Une checklist de 10 points à passer sur chaque libellé
- La formule Flesch FR + grille de niveaux (cible publique : F ≥ 70)
- Une méthode pas-à-pas pour reformuler un texte existant
- Les cas où il faut **déroger** (citation littérale, termes juridiques précis, voix de marque)

## Installation comme skill Claude Code

Un *skill* Claude Code est un fichier markdown auto-chargé quand le contexte de conversation déclenche sa description. Pour l'installer en global (utilisable dans n'importe quel projet) :

```bash
# macOS / Linux
mkdir -p ~/.claude/skills/langage-clair-fr
cp SKILL.md ~/.claude/skills/langage-clair-fr/
```

```powershell
# Windows
New-Item -ItemType Directory -Force "$HOME\.claude\skills\langage-clair-fr"
Copy-Item SKILL.md "$HOME\.claude\skills\langage-clair-fr\"
```

Claude détecte le skill à la prochaine session et le déclenche automatiquement sur les tâches de copy FR user-facing.

Pour un usage **projet-only** : placer le fichier dans `.claude/skills/langage-clair-fr/SKILL.md` à la racine du repo.

## Usage sans Claude Code

Le contenu de [`SKILL.md`](./SKILL.md) sert aussi de mémo autonome. Trois usages possibles :

- L'imprimer comme cheat-sheet de relecture
- Le coller en pré-prompt dans n'importe quel chatbot
- S'en servir comme grille de revue pour une équipe rédaction

## Licence

[MIT](./LICENSE). Réutilisation libre, attribution requise (conservation de la mention de copyright et du texte de licence dans toute redistribution).

Les référentiels cités (FALC, Langage Clair DITP, Plain Language, Flesch FR) sont des biens publics ou des standards ouverts.
