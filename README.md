# langage-clair-fr

Règles d'écriture en français pour produire des textes que des lecteurs non-experts comprennent **à la première lecture**, sans avoir à relire ni demander de l'aide.

Le fichier [`SKILL.md`](./SKILL.md) croise quatre référentiels publics :

- **FALC** : Facile à Lire et à Comprendre (Inclusion Europe, UNAPEI)
- **Langage Clair** : DITP / modernisation.gouv.fr
- **Plain Language** : tradition anglo-saxonne (PLAIN, plainlanguage.gov)
- **Flesch FR** : formule de lisibilité Kandel-Moles (1958)

## À qui ça s'adresse

Pensé pour les contextes où la clarté du texte est une **question d'équité d'accès**, pas un choix stylistique :

- Droit du travail, droits sociaux, démarches administratives
- Santé, éducation, services publics
- UI, emails transactionnels, FAQ pour grand public
- Vulgarisation de textes juridiques ou techniques

Ne s'applique **pas** à la doc dev interne, au marketing à effet stylistique, ni à la poésie.

## Ce que le document contient

- 10 règles non-négociables (une idée par phrase, voix active, verbes plutôt que noms, etc.)
- Un lexique de substitution **bureaucratique vers clair** (environ 25 entrées)
- Une liste d'anti-patterns FR fréquents
- Une checklist de 10 points à passer sur chaque libellé
- La formule Flesch FR + grille de niveaux (cible publique : F ≥ 70)
- Une méthode pas-à-pas pour reformuler un texte existant
- Les cas où il faut **déroger** (citation littérale, termes juridiques précis, voix de marque)

## Utilisation

Le fichier `SKILL.md` est un document markdown autonome, indépendant de tout outil. Trois usages possibles.

### 1. Charger dans un assistant IA de code

La plupart des assistants IA supportent le chargement de fichiers de règles externes. Quelques chemins connus :

| Outil | Emplacement |
|---|---|
| Aider | `aider --read SKILL.md`, ou clé `read:` dans `.aider.conf.yml` |
| Claude Code | `~/.claude/skills/langage-clair-fr/SKILL.md` |
| Codex CLI (OpenAI) | inclure le contenu dans le fichier `AGENTS.md` à la racine du projet |
| Continue.dev | référencer le fichier dans la section `rules` de `~/.continue/config.json` |
| Cursor | `.cursor/rules/langage-clair-fr.mdc` à la racine du projet |

Consulter la documentation de l'outil pour la syntaxe de chargement exacte. La syntaxe évolue : ces chemins sont indicatifs.

### 2. Comme prompt système d'une interface chat

Coller le contenu de `SKILL.md` dans :

- Le champ « Instructions » d'un GPT personnalisé (ChatGPT) ou d'un Projet (Claude.ai, Le Chat de Mistral)
- Le system prompt d'une intégration API (OpenAI, Anthropic, Mistral, Gemini, Llama, etc.)
- Le premier message d'une conversation, en précisant : « Voici les règles à appliquer dans nos échanges. »

Le contenu fonctionne avec n'importe quel modèle suffisamment compétent en français.

### 3. Comme document autonome

- Imprimer comme cheat-sheet de relecture
- Servir de grille de revue pour une équipe rédaction
- Citer ou adapter dans un guide interne de rédaction

## Licence

[MIT](./LICENSE). Réutilisation libre, attribution requise (conservation de la mention de copyright et du texte de licence dans toute redistribution).

Les référentiels cités (FALC, Langage Clair DITP, Plain Language, Flesch FR) sont des biens publics ou des standards ouverts.

## Contribuer

Issues et pull requests bienvenues, en particulier pour :

- Compléter le lexique de substitution
- Ajouter des anti-patterns rencontrés en production
- Corriger des erreurs ou imprécisions sur les référentiels cités
- Traduire ou adapter pour d'autres langues
