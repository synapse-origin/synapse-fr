# 🎯 Intent — Intention stratégique

Cette page complète [SYNAPSE-V1.md](SYNAPSE-V1.md), [roles.md](roles.md) et [loops.md](loops.md) en clarifiant un concept central du framework : **l'Intent**.

L'Intent est ce que toute l'organisation cherche à servir. Il est porté par l'**Intent Architect**, vérifié par l'**Intent Sync**, mesuré par la métrique **Clarté d'intention**.

---

## Qu'est-ce qu'un Intent ?

Un Intent (ou Intent Statement) est une déclaration formelle qui répond à **trois questions** :

1. **Que cherchons-nous à accomplir ?** (Objectives mesurables)
2. **Qu'est-ce que nous ne ferons pas ?** (Out-of-Scope)
3. **Sous quelles contraintes ?** (Constraints — légales, éthiques, ressources, etc.)

Il est complété par : un **contexte stratégique** (le « pourquoi maintenant »), des **stakeholders**, des **principes de décision** explicites, et des **critères de succès** observables.

L'Intent n'est pas un plan d'action. C'est la **boussole** qui permet d'évaluer après coup si une décision a servi ou non l'intention.

---

## Hiérarchie des Intents

SYNAPSE distingue deux niveaux d'Intent, qui scalent avec la taille de l'organisation.

### Niveau 1 — Org Intent (`level: ORGANIZATION`)

L'**Intent unique de l'organisation entière**. C'est le « north star ».

**Règle fondatrice** : il y a **un seul Org Intent ACTIVE** à un instant donné par organisation. Les versions antérieures existent en parallèle avec le statut `SUPERSEDED` (chaîne de versioning), mais une seule fait foi à l'instant T.

**Pourquoi le singleton ?** Parce que l'alignement cognitif que SYNAPSE promet repose sur une référence unique. Si trois Org Intents coexistaient, le score d'alignement d'une Decision perdrait son sens (alignée avec laquelle ?). Plusieurs « directions stratégiques » ne sont pas plusieurs Intents — ce sont plusieurs **Objectives** à l'intérieur d'un même Intent.

### Niveau 2 — Team Intent (`level: TEAM`)

Un Intent porté par une **équipe identifiable** au sein de l'organisation. Il décline l'Org Intent sur le périmètre de cette équipe.

**Règle fondatrice** : un Team Intent **doit** référencer une `Team` existante de la même organisation. Il n'y a pas de Team Intent orphelin — pas de « Team Intent fictif » qui annoncerait une équipe future. Si vous n'avez pas encore d'équipes, vous n'avez pas besoin de Team Intents (cf. section suivante).

Un Team Intent hérite (par défaut) des Constraints et Out-of-Scope de l'Org Intent. Ses Objectives sont propres à l'équipe et doivent rester cohérents avec ceux du parent — la **cohérence** est vérifiée à la création (coherence check).

---

## Quand utiliser Org Intent vs Team Intent ?

La question revient à demander : **« Avons-nous des équipes distinctes qui se distribuent la responsabilité stratégique ? »**

### Solo-dev ou petite organisation (1-5 personnes)

Une seule personne (ou un petit groupe) porte toute la stratégie. Aucune équipe formalisée.

→ **Un seul Org Intent**. Vos axes stratégiques sont des **Objectives** dans cet Intent. Pas de Team Intent.

Exemple :

```
Org Intent : « Établir SYNAPSE comme cadre de référence post-agile pour l'ère IA »
  ├─ Objective 1 : Plateforme de référence opérable
  ├─ Objective 2 : Rayonnement & vocabulaire adopté
  └─ Objective 3 : Dogfooding & boucle de feedback continue
```

### Organisation avec équipes formalisées (10+ personnes, plusieurs équipes)

Chaque équipe a une responsabilité stratégique distincte qu'elle pilote au quotidien.

→ **Un Org Intent + N Team Intents**, chacun rattaché à une Team. Les Objectives de l'Org Intent deviennent des Team Intents quand une équipe les prend en charge.

Exemple :

```
Org Intent : « Devenir la référence européenne du framework de collaboration humain-IA »
  ├─ Team Intent (Engineering)        → portée par la Team « Plateforme »
  ├─ Team Intent (DevRel)             → portée par la Team « Communauté »
  └─ Team Intent (Quality/SRE)        → portée par la Team « Qualité »
```

### Transition solo → multi-team

Quand votre organisation grandit et que vous instanciez vos premières équipes, le chemin canonique est :

1. Créer une `Team` dans SYNAPSE
2. **Promouvoir** un Objective de l'Org Intent en Team Intent rattaché à cette équipe
3. L'Objective de l'Org Intent devient soit le titre de ce Team Intent, soit son premier Objective interne
4. Les Constraints sont héritées par défaut

Cette ergonomie de transition est ce qui distingue SYNAPSE d'un framework figé : il **grandit avec l'organisation**, sans demander de tout réécrire à chaque étape.

---

## Confusion fréquente : Objectives vs Team Intents

C'est la confusion la plus courante chez les utilisateurs débutants.

| | Objectives (dans un Intent) | Team Intents |
|---|---|---|
| **Représente** | Un axe / une dimension stratégique | La responsabilité d'une équipe |
| **Propriété** | Un seul propriétaire (porteur de l'Intent) | Une équipe distincte |
| **Quand l'utiliser** | Toujours, dès le premier Intent | Quand des équipes existent réellement |
| **Solo-dev** | ✅ Plusieurs Objectives par Intent | ❌ Évitez les Team Intents |
| **Multi-team** | ✅ Plusieurs Objectives par Intent | ✅ Un Team Intent par équipe |

**Règle de décision** : si la réponse à « qui porte cet axe ? » est la même personne / le même groupe que pour les autres axes, c'est un Objective. Si la réponse est une équipe différente avec sa propre dynamique, c'est un Team Intent.

---

## Cycle de vie d'un Intent

Un Intent passe par les statuts suivants :

| Statut | Sens | Modifiable ? |
|--------|------|--------------|
| `DRAFT` | Brouillon, en cours de rédaction | ✅ Oui, en place |
| `ACTIVE` | En vigueur, fait référence pour les Decisions | Révision uniquement (versioning) |
| `SUPERSEDED` | Remplacé par une version plus récente | ❌ Immuable (historique) |
| `ARCHIVED` | Plus pertinent (ex: pivot complet) | ❌ Immuable |

**Révision (versioning)** : un Intent ACTIVE ne se modifie pas en place. On en crée une nouvelle version (v2, v3…) qui passe ACTIVE, et la précédente passe SUPERSEDED via la chaîne `previousVersionId`. Cela préserve la traçabilité — toute Decision passée reste rattachée à la version de l'Intent en vigueur au moment où elle a été prise.

**Pourquoi ne pas modifier en place ?** Parce que l'Intent est le contrat avec lequel les Decisions sont évaluées (alignement, scoring). Le réécrire silencieusement reviendrait à réécrire l'histoire — antithétique au principe de transparence cognitive.

---

## Intégration avec les autres composants SYNAPSE

| Composant | Rôle vis-à-vis de l'Intent |
|-----------|---------------------------|
| **Intent Architect** | Porte la rédaction, l'évolution et le veto sur les Decisions qui dérivent de l'intention |
| **Intent Sync** (boucle hebdo) | Vérifie l'alignement de l'organisation avec l'Intent. Déclenche révision si dérive structurelle |
| **Memory Agent** | Stocke les Decisions reliées à l'Intent — quand aucune Decision ne référence un Intent, c'est un signal de drift |
| **Pattern Agent** | Détecte les patterns qui contredisent l'Intent (ex: décisions répétées hors-scope) |
| **Métrique « Clarté d'intention »** | Mesure (>80% cible) la proportion des collaborateurs qui peuvent restituer l'Intent fidèlement |

---

## Anti-patterns à éviter

❌ **Multiplier les Org Intents pour porter plusieurs axes stratégiques.** → Utilisez les Objectives. Le singleton n'est pas une contrainte arbitraire, c'est le fondement du scoring d'alignement.

❌ **Créer des Team Intents sans Team correspondante.** → Soit créez la Team d'abord, soit restez sur des Objectives au niveau Org Intent. Un Team Intent orphelin confond l'auto-rattachement des Decisions et brouille la lecture de la hiérarchie.

❌ **Modifier un Intent ACTIVE en place.** → Toujours créer une nouvelle version (révision). La perte de traçabilité est irrémédiable.

❌ **Rédiger un Intent vague ou tautologique** (« Être les meilleurs », « Servir nos clients »). → Un Intent doit produire des Decisions évaluables. Si toute Decision est compatible avec l'Intent, l'Intent ne sert à rien.

❌ **Reformuler l'Intent à chaque review hebdo.** → Une révision est un événement structurant, pas une activité courante. Si l'Intent change toutes les semaines, c'est un signe que la stratégie n'est pas stabilisée — résolvez ce problème avant de poursuivre.

---

## Voir aussi

- [Les 4 rôles humains](roles.md) — notamment Intent Architect
- [Les 3 boucles](loops.md) — notamment Intent Sync
- [Les 11 métriques](metrics.md) — notamment Clarté d'intention
- [Vue d'ensemble](SYNAPSE-V1.md)
