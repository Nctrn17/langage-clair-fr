---
name: langage-clair-fr
description: Écriture FR accessible pour publics non-experts (salariés, ayants droit, demandeurs, personnes en situation de handicap cognitif, public administratif). Croise FALC (Inclusion Europe / UNAPEI), Langage Clair (DITP / modernisation.gouv.fr), Plain Language internationale et la recherche en lisibilité (Flesch FR adapté Kandel-Moles). À déclencher quand on écrit, relit ou modifie du texte FR user-facing — libellés UI, emails transactionnels, FAQ, messages d'erreur, copy onboarding, vulgarisation administrative ou juridique. Ne pas déclencher sur la doc dev interne, le marketing à effet stylistique, la poésie.
---

# Langage clair FR — règles d'écriture accessible

Outil pour écrire en français des textes que des lecteurs non-experts comprennent **à la première lecture**, sans devoir relire ni demander de l'aide. S'applique en priorité aux secteurs où le langage clair est une question d'**équité d'accès** : droit du travail, droits sociaux, démarches administratives, santé, éducation, services aux usagers.

## Quand utiliser ce skill

- Rédiger ou modifier une chaîne UI affichée à un utilisateur (label, bouton, helper, error, empty state)
- Écrire une page d'onboarding, une FAQ, un email transactionnel
- Vulgariser un texte juridique, administratif ou technique
- Reformuler un message d'erreur écrit par un développeur ou copié du droit
- Faire une revue de copy avant merge / déploiement

## Quand ne PAS utiliser ce skill

- Commentaires de code ou documentation technique pour développeurs
- Texte marketing où la signature de marque demande une figure de style
- Citation littérale d'un texte de loi (le texte doit rester intact, c'est la *paraphrase* qui s'applique)
- Contenu interne entre experts d'un même métier

## Référentiels croisés

| Source | Origine | Apport principal |
|---|---|---|
| **FALC** — Facile à Lire et à Comprendre | Inclusion Europe, UNAPEI (FR), standard EU | Méthodologie d'écriture pour public en situation de handicap cognitif. Validée par des "relecteurs" co-concepteurs. Règles strictes sur syntaxe et vocabulaire. |
| **Langage Clair** | DITP / modernisation.gouv.fr | Adaptation française du Plain Language. Pour réécrire le langage administratif. Focus : démarche citoyenne. |
| **Plain Language** | International (PLAIN, plainlanguage.gov, Inkpot UK) | Tradition anglo-saxonne. Recherche empirique sur la compréhension. |
| **Flesch FR (Kandel-Moles 1958)** | Recherche linguistique | Score quantitatif de lisibilité, adapté du Flesch-Kincaid pour le français. Outil web : **scolarius.com**. |
| **FALC validation par pairs** | UNAPEI, Inclusion Europe | Le texte n'est "validé FALC" que s'il a été relu par une personne du public cible qui peut le reformuler en ses mots. |

## Règles non-négociables

### 1. Une idée par phrase

❌ « Vous devez fournir votre fiche de paie qui doit être lisible et datée de moins de 3 mois pour que nous puissions traiter votre demande, sauf si vous êtes en CDD auquel cas le contrat suffit. »

✅ « Joignez votre fiche de paie. Elle doit être lisible et dater de moins de 3 mois. Si vous êtes en CDD, votre contrat suffit. »

### 2. Phrase courte — viser 15 mots, plafonner à 20

Au-delà de 25 mots, la phrase devient difficile à mémoriser pendant la lecture. Couper aux conjonctions (« et », « mais », « car », « parce que », « cependant »).

### 3. Voix active

❌ « Votre dossier sera examiné par nos services dans un délai de 15 jours. »

✅ « Nous examinons votre dossier sous 15 jours. »

La voix passive masque qui fait quoi. En administration française, c'est endémique.

### 4. Verbes plutôt que noms — pas de nominalisations administratives

❌ « la réalisation de votre démarche », « la mise en œuvre du dispositif », « l'application des règles »

✅ « réaliser votre démarche », « appliquer le dispositif », « appliquer les règles »

Une nominalisation transforme un verbe en nom abstrait. Elle vide la phrase de son sujet et de son temps.

### 5. Vocabulaire concret — pas de jargon, pas de figures

- Pas de métaphores (« naviguer dans votre espace », « franchir une étape »)
- Pas d'abstractions vagues (« dans le cadre de », « au titre de », « à ce stade »)
- Pas de sigles non explicités à la première occurrence
- Préférer le mot du quotidien au mot juridique quand les deux existent

### 6. Cohérence terminologique

Mêmes mots pour mêmes choses, **toujours**. Si tu commences à parler de « votre fiche de paie », ne bascule pas en cours de page sur « bulletin de salaire » ou « relevé de paie ». La variation stylistique tue la compréhension.

### 7. Présent de l'indicatif

Éviter conditionnel et subjonctif quand l'indicatif suffit.

❌ « Il conviendrait que vous joigniez votre RIB. »
✅ « Joignez votre RIB. »

### 8. Pas de double négation

❌ « Il n'est pas impossible que vous ne soyez pas éligible. »
✅ « Vous êtes peut-être éligible. Vérifiez avec votre syndicat. »

### 9. Adresse personnelle directe

Choisir et tenir : **vous** (administratif neutre, le plus courant), **tu** (proximité, à éviter en B2C grand public sauf jeunesse), **on** + **vous** (notre service + l'utilisateur, registre moderne — beta.gouv.fr, Pass Culture).

Pas de « le bénéficiaire », « l'usager », « le demandeur » à la troisième personne — c'est froid et déresponsabilisant.

### 10. Listes plutôt que paragraphes denses

Une énumération de plus de 2 éléments → liste à puces. Surtout pour les pièces à fournir, les étapes à suivre, les conditions à remplir.

## Lexique de substitution — bureaucratique → clair

| ❌ Tournure administrative | ✅ Équivalent clair |
|---|---|
| afin de | pour |
| au titre de / à titre de | pour / comme |
| dans le cadre de | pour / en |
| dans la mesure où | si / parce que |
| il convient de / il y a lieu de | vous devez / il faut |
| il est porté à votre connaissance que | nous vous informons que (ou : ø, et on dit le fait directement) |
| en effet | (souvent supprimable) |
| effectuer | faire |
| diligenter | lancer / faire |
| s'avérer | être |
| nonobstant | malgré |
| préalablement | avant |
| ultérieurement | après / plus tard |
| antérieurement | avant |
| postérieurement | après |
| à compter de | à partir de |
| en sus de | en plus de |
| nonobstant | malgré |
| au-delà du / en deçà du | plus de / moins de |
| ledit / ladite / lesdits | ce / cette / ces |
| consécutivement | après / ensuite |
| susceptible de | qui peut |
| constituer un dossier | rassembler vos pièces |
| pièces justificatives | justificatifs |
| saisir l'administration / la justice | contacter / s'adresser à |
| solliciter | demander |
| accuser réception | confirmer la réception |
| déposer une demande | demander |

## Anti-patterns FR fréquents

### Le "Il convient de..." passif

❌ « Il convient de procéder à la vérification des éléments transmis. »
✅ « Vérifiez les éléments que vous avez transmis. » (ou : « Nous vérifions… »)

### Le conditionnel de politesse abusif

❌ « Vous seriez susceptible de bénéficier d'un complément. »
✅ « Vous pouvez peut-être recevoir un complément. »

### L'empilement de prépositions

❌ « Dans le cadre de la mise en œuvre du dispositif d'accompagnement au titre de l'année 2026… »
✅ « Pour appliquer l'accompagnement 2026… »

### Le sujet caché derrière « il »

❌ « Il vous sera demandé de vous présenter. »
✅ « Nous vous demandons de venir. » / « Vous devez venir. »

### Le double sens du "ou"

« Pour les salariés du privé ou du public et leurs ayants droit » — ambigu : et/ou ?

✅ Reformuler explicitement : « Pour les salariés du privé. Pour les salariés du public. Pour leurs ayants droit. »

### Le sigle non explicité

❌ « CMU-C, AME, ACS, RSA, CPAM » sans définition à la première occurrence
✅ Première occurrence : nom complet + sigle entre parenthèses. Occurrences suivantes : sigle seul.

### La date romaine ou la date en chiffres dans une phrase

❌ « le 1er trimestre de 2026 »
✅ « entre janvier et mars 2026 » (préférer le mot quand on parle d'une période)

## Checklist rapide — passer chaque libellé à travers

À chaque libellé UI / message / paragraphe à publier :

1. ☐ La phrase la plus longue fait-elle ≤ 20 mots ?
2. ☐ Toutes les phrases sont-elles à la voix active ?
3. ☐ Y a-t-il une nominalisation que je peux remplacer par un verbe ?
4. ☐ Toutes les abréviations sont-elles explicitées à la 1ère occurrence ?
5. ☐ Le sujet de chaque action est-il explicite ? (« nous », « vous », pas « il »)
6. ☐ Le même objet est-il toujours nommé du même mot ?
7. ☐ Y a-t-il un mot du quotidien plus court pour ce mot administratif ?
8. ☐ Si on me lit à voix haute, comprends-je tout à la première écoute ?
9. ☐ Y a-t-il un mot que mon père / ma grand-mère / un ado de 14 ans ne connaîtrait pas ?
10. ☐ Le texte tient-il sans bagage juridique / professionnel particulier ?

## Comment scorer

### Score Flesch FR (Kandel-Moles)

```
F = 207 − 1,015 × (mots / phrases) − 73,6 × (syllabes / mots)
```

| Score F | Niveau | Public visé |
|---|---|---|
| ≥ 80 | Très facile | Tout public, lecture rapide |
| 70 – 80 | Facile | Collège, public administratif large |
| 60 – 70 | Standard | Lycée / adulte courant |
| 50 – 60 | Plutôt difficile | Bac+, lecture appliquée |
| < 50 | Difficile | Spécialiste / lecture attentive |

**Cible pour usage public** (administration, social, services) : **F ≥ 70**.

Outil web : **scolarius.com** (copier-coller, score instantané).

### Validation FALC

Le texte n'est validé FALC que si un **relecteur du public cible** (= une personne de la population à qui le texte s'adresse, formée à la relecture FALC) peut :

1. Lire le texte une seule fois sans s'arrêter
2. Le reformuler dans ses propres mots
3. Trouver l'information qu'il cherche dans la page

Pour les organisations sociales et publiques, un panel de relecteurs FALC peut être commandité auprès d'UNAPEI ou de structures spécialisées.

## Quand DÉROGER

- **Citation littérale d'un texte de loi** : on cite tel quel, on vulgarise à côté.
- **Termes juridiques précis qui ont des conséquences** : si « rupture conventionnelle » et « démission » ont des conséquences différentes, on garde les deux termes — on les explique.
- **Voix de marque assumée** : un acteur jeunesse peut tutoyer, une marque éditoriale peut allonger une phrase pour le rythme. Conscience > réflexe.
- **Public d'experts** : la simplification entre soi (médecins entre médecins, juristes entre juristes) tue la précision.

## Méthode pour reformuler rapidement

Quand un texte existant est à simplifier :

1. **Identifier le verbe principal** de chaque phrase. S'il est masqué dans une nominalisation, le ramener à la surface.
2. **Identifier le sujet** : qui fait l'action ? Si « il » impersonnel ou voix passive, expliciter.
3. **Couper aux conjonctions** si la phrase dépasse 20 mots. Une phrase = une idée.
4. **Substituer le vocabulaire administratif** par les équivalents du quotidien (cf table ci-dessus).
5. **Tester à voix haute** : si on butte, on simplifie encore.
6. **Comparer le score Scolarius** avant/après.

## Sources & lectures

- **UNAPEI — Information pour tous** : [unapei.org](https://www.unapei.org) → ressources FALC
- **Inclusion Europe — Information for all** : manuel européen de référence FALC
- **DITP — Plan langage clair** : [modernisation.gouv.fr](https://www.modernisation.gouv.fr) (chercher « langage clair »)
- **Scolarius** : [scolarius.com](https://scolarius.com) — score de lisibilité FR instantané
- **plainlanguage.gov** : référentiel Plain Language US, principes transposables
- **PLAIN — Plain Language Action and Information Network** : standards internationaux
- **LanguageTool** : [languagetool.org](https://languagetool.org) — vérif grammaire + style en FR, plugins éditeurs
- **Antidote** (payant) : section « Lisibilité »
- Recherche : Kandel & Moles (1958) — adaptation Flesch pour le français
- Recherche : Mesnager (2002) sur la lisibilité scolaire FR
