# 🤖 Les 4 Agents IA dans SYNAPSE

Les agents IA de SYNAPSE ne remplacent pas les humains. Ils **augmentent** leur capacité à comprendre, décider et agir dans un système complexe.

---

## Vue d'Ensemble

| Agent | Mission | Déclenchement |
|-------|---------|---------------|
| **Memory Agent** 🧠 | Mémoire organisationnelle | Continu |
| **Pattern Agent** 🔍 | Détection de récurrences | Continu + alertes |
| **Simulation Agent** 🎲 | Anticipation des décisions | À la demande |
| **Coordination Agent** 🔗 | Optimisation des flux | Continu + proactif |

---

## 🧠 Memory Agent

### Mission

Être la **mémoire parfaite** de l'organisation. Capturer, structurer et restituer la connaissance collective.

### Le Problème qu'il Résout

> "On avait déjà essayé ça il y a 6 mois, mais personne ne s'en souvient..."

Les organisations perdent leur mémoire : les décisions sont oubliées, le contexte se perd avec le turnover, les mêmes erreurs se répètent.

### Ce qu'il Fait

**Capture automatique**
- Enregistre chaque décision formalisée
- Extrait les entités clés (personnes, projets, technologies)
- Construit un graphe de connaissances interconnecté

**Recherche contextuelle**
- Retrouve les décisions similaires passées
- Fournit le contexte historique pertinent
- Répond à "Qu'avions-nous décidé sur ce sujet ?"

**Détection de contradictions**
- Identifie quand une nouvelle décision contredit une ancienne
- Alerte pour clarifier ou justifier le changement
- Maintient la cohérence organisationnelle

### Exemple de Cas d'Usage

L'équipe débat sur le choix d'une base de données. Memory Agent intervient :

> "Il y a 8 mois, un débat similaire a eu lieu (Décision #089). PostgreSQL avait été choisi pour le support des transactions. Résultat : positif, aucun problème rencontré depuis."

L'équipe gagne 2h de discussion et évite de refaire les mêmes analyses.

### Bénéfices Mesurables

- Réduction du temps de recherche d'information
- Moins de décisions contradictoires
- Onboarding accéléré (la mémoire persiste malgré le turnover)

---

## 🔍 Pattern Agent

### Mission

Identifier les **récurrences** — bonnes ou mauvaises — dans le comportement de l'organisation.

### Le Problème qu'il Résout

> "On découvre en rétro qu'on a le même blocage depuis 3 mois..."

Les patterns émergent lentement et sont détectés trop tard, souvent en rétrospective quand le mal est fait.

### Ce qu'il Fait

**Détection de patterns négatifs**
- Blocages récurrents sur les mêmes étapes
- Goulots d'étranglement systématiques
- Dépassements d'estimation répétés

**Détection de patterns positifs**
- Pratiques qui fonctionnent mieux que d'autres
- Configurations d'équipe efficaces
- Succès reproductibles

**Alertes temps réel**
- Notification dès qu'un seuil est franchi
- Pas besoin d'attendre la prochaine rétro
- Action corrective immédiate possible

### Exemple de Cas d'Usage

Pattern Agent détecte :

> "Les features impliquant l'API de paiement prennent systématiquement 2x le temps estimé. 5 occurrences en 2 mois. Cause probable : intégration externe complexe."

L'équipe ajuste ses estimations et prévoit un buffer pour ce type de feature.

### Bénéfices Mesurables

- Détection 10x plus rapide que les méthodes manuelles
- Réduction des blocages récurrents
- Capitalisation sur les bonnes pratiques

---

## 🎲 Simulation Agent

### Mission

**Anticiper** les conséquences des décisions majeures avant de les prendre.

### Le Problème qu'il Résout

> "On a foncé sur cette décision, et 3 mois plus tard on se rend compte qu'on aurait dû faire autrement..."

Les décisions importantes sont souvent prises avec peu de visibilité sur leurs conséquences à moyen terme.

### Ce qu'il Fait

**Génération de scénarios**
- Produit 3 à 5 scénarios réalistes pour chaque décision
- Estime les probabilités de succès
- Identifie les risques spécifiques à chaque option

**Analyse contextuelle**
- S'appuie sur l'historique (Memory Agent)
- Prend en compte les décisions similaires passées
- Apprend des succès et échecs précédents

**Recommandation argumentée**
- Suggère le scénario optimal
- Explique le raisonnement
- Indique le niveau de confiance

### Exemple de Cas d'Usage

Décision : "Faut-il migrer vers une architecture microservices ?"

Simulation Agent génère :
- **Scénario A** : Migration complète en 6 mois — 60% de chances de succès, risque principal sur la migration BDD
- **Scénario B** : Migration progressive en 12 mois — 80% de chances de succès, risques distribués
- **Scénario C** : Optimisation de l'existant — 95% de succès, mais ne résout pas le problème long terme

Recommandation : Scénario B, meilleur équilibre risque/bénéfice.

### Bénéfices Mesurables

- Décisions mieux informées
- Réduction des "mauvaises surprises"
- Apprentissage continu (comparaison prédiction vs réalité)

---

## 🔗 Coordination Agent

### Mission

Optimiser les **flux** de travail et d'information. Identifier les blocages avant qu'ils ne ralentissent l'équipe.

### Le Problème qu'il Résout

> "J'attends cette review depuis 3 jours, et personne ne savait que c'était bloquant..."

La coordination humaine a ses limites : les dépendances sont mal visibles, les blocages sont signalés trop tard, les réunions de synchronisation consomment du temps.

### Ce qu'il Fait

**Détection de blocages**
- Identifie les tâches en attente trop longtemps
- Repère les dépendances critiques
- Alerte avant que le blocage n'impacte les délais

**Suggestions d'intervention**
- Propose des réassignations si quelqu'un est surchargé
- Suggère des priorisations alternatives
- Identifie les opportunités de parallélisation

**Optimisation proactive**
- Analyse le graphe de dépendances
- Détecte les goulots potentiels
- Suggère des reconfigurations d'équipe temporaires

### Exemple de Cas d'Usage

Coordination Agent détecte :

> "La PR de PersonneX attend une review depuis 2h. PersonneY (reviewer assigné) a 8 autres PR en attente et part en congés demain. PersonneZ est disponible et compétente sur ce domaine."

Suggestion : réassigner la review à PersonneZ.

Résultat : blocage résolu en 30 minutes au lieu de 3 jours.

### Bénéfices Mesurables

- Réduction drastique des temps de blocage
- Moins de temps passé en réunions de synchronisation
- Meilleure visibilité sur les dépendances

---

## 🔄 Interactions Entre Agents

Les 4 agents ne fonctionnent pas en silo. Ils collaborent :

- **Memory** alimente **Pattern** avec l'historique
- **Pattern** informe **Simulation** des récurrences connues
- **Simulation** aide **Coordination** à prioriser
- **Coordination** déclenche des **Decision Moments** si nécessaire

---

## ⚖️ Principes de Conception

### L'IA propose, l'humain décide

Aucun agent ne prend de décision à la place des humains. Ils fournissent de l'information, des alertes, des suggestions — jamais des ordres.

### Transparence totale

Chaque proposition d'un agent est explicable. Les humains peuvent toujours demander "pourquoi cette suggestion ?" et obtenir une réponse claire.

### Dégradation gracieuse

Si un agent dysfonctionne, les autres continuent. Le système est résilient et peut fonctionner en mode dégradé.

### Amélioration continue

Les agents apprennent des retours. Quand une suggestion est refusée ou qu'une prédiction s'avère fausse, le système s'ajuste.

---

## 📊 Métriques de Valeur

| Agent | Métrique Clé | Impact Typique |
|-------|--------------|----------------|
| Memory | Temps de recherche d'info | -50% |
| Pattern | Délai de détection des problèmes | 10x plus rapide |
| Simulation | Qualité des décisions | +30% de succès |
| Coordination | Temps de blocage | -70% |

*Ces métriques sont des ordres de grandeur basés sur les objectifs du framework, les résultats varient selon le contexte.*

---

## 🚀 Accès aux Agents

Les agents SYNAPSE sont disponibles via :

**SYNAPSE Cloud** *(bientôt disponible)*
- Agents hébergés et maintenus
- Mise en route rapide
- Tarification à l'usage

**SYNAPSE Enterprise**
- Déploiement sur votre infrastructure
- Souveraineté totale des données
- Support dédié

**Organisation Pilote**
- Accès anticipé
- Co-construction
- Conditions préférentielles

📧 Contact : synapse-origin@proton.me

---

## 📚 Voir Aussi

- [Vue d'ensemble SYNAPSE](SYNAPSE-V1.md)
- [Les 4 rôles humains](roles.md)
- [Les 3 boucles](loops.md)
- [Les 11 métriques](metrics.md)
- [Charte éthique](ethics.md)

---

*Documentation SYNAPSE — Janvier 2026*
