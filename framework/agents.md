# 🤖 Les 4 Agents Cognitifs SYNAPSE

Les agents SYNAPSE ne remplacent pas les humains. Ils **augmentent** leur capacité à comprendre, décider et agir dans un système complexe.

**Principe fondamental :** L'agent propose, l'humain décide. Toujours.

---

## Vue d'Ensemble

| Agent | Mission | Déclenchement | Rôle humain principal |
|-------|---------|---------------|----------------------|
| **Memory** 🧠 | Mémoire organisationnelle | Continu | Tous |
| **Pattern** 🔍 | Détection de récurrences | Continu + alertes | System Orchestrator |
| **Simulation** 🎲 | Anticipation des décisions | À la demande | Intent Architect |
| **Coordination** 🔗 | Optimisation des flux | Continu + proactif | System Orchestrator |

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

### Ce qu'il ne Doit PAS Faire

| Interdit | Raison |
|----------|--------|
| ❌ Capturer des conversations privées sans consentement | Protection vie privée |
| ❌ Enregistrer des données personnelles sensibles (santé, opinions politiques) | RGPD |
| ❌ Modifier ou supprimer des décisions sans trace | Intégrité de l'historique |
| ❌ Fournir des informations à des personnes non autorisées | Confidentialité |
| ❌ Interpréter ou juger les décisions passées | Neutralité |

### Exemples de Prompts

```
💬 "Qu'avons-nous décidé concernant [sujet] ?"
💬 "Qui a travaillé sur [projet] et quelles étaient les conclusions ?"
💬 "Y a-t-il des décisions passées qui contredisent [proposition] ?"
💬 "Quel était le contexte de la décision #[ID] ?"
💬 "Quelles technologies avons-nous évaluées pour [besoin] ?"
💬 "Montre-moi l'historique des décisions sur [domaine] ces 6 derniers mois"
```

### Configuration (System Orchestrator)

| Paramètre | Description | Valeur par défaut |
|-----------|-------------|-------------------|
| Sources de capture | Quels canaux sont enregistrés | Décisions formelles uniquement |
| Rétention | Durée de conservation | Illimitée |
| Niveau d'extraction | Profondeur d'analyse des entités | Moyen |
| Accès | Qui peut interroger | Tous les rôles SYNAPSE |

### Métriques de Succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Taux de réutilisation | > 40% des décisions s'appuient sur l'historique | Questionnaire décideurs |
| Temps de recherche | < 2 min pour trouver une info | Logs de requêtes |
| Contradictions détectées | 100% des contradictions majeures | Audit mensuel |

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

**Alertes contextualisées**
- Notification quand un seuil est franchi
- Données chiffrées à l'appui
- Suggestions d'actions (pas d'ordres)

### Ce qu'il ne Doit PAS Faire

| Interdit | Raison |
|----------|--------|
| ❌ Comparer les performances individuelles | Pas de flicage |
| ❌ Alerter plus de 5 fois par jour (sauf critique) | Éviter l'alert fatigue |
| ❌ Détecter des patterns sur moins de 3 occurrences | Éviter les faux positifs |
| ❌ Attribuer la responsabilité d'un pattern à une personne | Approche systémique, pas blame |
| ❌ Proposer des actions RH (licenciement, sanction) | Hors périmètre éthique |

### Exemples de Prompts

```
💬 "Quels patterns négatifs as-tu détectés ce mois-ci ?"
💬 "Y a-t-il des blocages récurrents sur [projet/équipe] ?"
💬 "Quelles bonnes pratiques émergent des données ?"
💬 "Pourquoi les estimations sur [type de tâche] sont-elles souvent dépassées ?"
💬 "Compare les temps de cycle entre [période A] et [période B]"
💬 "Quels sont les 3 patterns les plus impactants actuellement ?"
```

### Configuration (System Orchestrator)

| Paramètre | Description | Valeur par défaut |
|-----------|-------------|-------------------|
| Seuil de détection | Nombre d'occurrences minimum | 3 |
| Fréquence d'analyse | À quelle fréquence scanner | Continue |
| Seuil d'alerte | Quand notifier | Impact > moyen |
| Max alertes/jour | Limite anti-spam | 5 |
| Canaux de notification | Où envoyer les alertes | Slack + email System Orchestrator |

### Métriques de Succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Taux de faux positifs | < 20% | Patterns ignorés / total |
| Délai de détection | < 1 semaine vs rétro classique | Timestamp première occurrence → alerte |
| Taux d'action | > 60% des patterns mènent à une action | Suivi des Pattern Reviews |

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
- Prend en compte les patterns connus (Pattern Agent)
- Apprend des succès et échecs précédents

**Recommandation argumentée**
- Suggère le scénario optimal
- Explique le raisonnement
- Indique le niveau de confiance

### Ce qu'il ne Doit PAS Faire

| Interdit | Raison |
|----------|--------|
| ❌ Présenter une recommandation comme une certitude | Humilité épistémique |
| ❌ Simuler des décisions RH individuelles | Éthique |
| ❌ Cacher les hypothèses sous-jacentes | Transparence |
| ❌ Ignorer les options proposées par les humains | Respect de l'autonomie |
| ❌ Refuser de simuler un scénario "parce qu'il est mauvais" | Neutralité |

### Exemples de Prompts

```
💬 "Simule les options pour [décision à prendre]"
💬 "Quels sont les risques si on choisit [option A] ?"
💬 "Compare [option A] vs [option B] sur 6 mois"
💬 "Quel est ton niveau de confiance sur cette recommandation ?"
💬 "Quelles hypothèses as-tu utilisées pour ce scénario ?"
💬 "Que s'est-il passé dans des situations similaires par le passé ?"
💬 "Ajoute un scénario où [contrainte supplémentaire]"
```

### Configuration (System Orchestrator)

| Paramètre | Description | Valeur par défaut |
|-----------|-------------|-------------------|
| Nombre de scénarios | Combien de scénarios générer | 3-5 |
| Horizon temporel | Sur quelle durée simuler | 6 mois |
| Sources de données | Quelles données utiliser | Memory + Pattern + externes |
| Seuil de confiance minimum | En dessous, avertir explicitement | 50% |

### Métriques de Succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Précision des prédictions | Écart < 20% | Comparaison prédiction vs réalité à M+3 |
| Utilisation | > 80% des décisions majeures simulées | Logs |
| Satisfaction décideurs | > 7/10 | Questionnaire post-décision |

---

## 🔗 Coordination Agent

### Mission

Optimiser les **flux** de travail et d'information. Identifier les blocages avant qu'ils ne ralentissent l'équipe.

### Le Problème qu'il Résout

> "J'attends cette review depuis 3 jours, et personne ne savait que c'était bloquant..."

La coordination humaine a ses limites : les dépendances sont mal visibles, les blocages sont signalés trop tard, les réunions de synchronisation consomment du temps.

### Ce qu'il Fait

**Détection de blocages**
- Se connecte aux outils (Jira, GitHub, Linear, etc.)
- Identifie les tâches en attente trop longtemps
- Repère les dépendances critiques
- Alerte avant que le blocage n'impacte les délais

**Suggestions d'intervention**
- Propose des réassignations si quelqu'un est surchargé
- Suggère des priorisations alternatives
- Identifie les opportunités de parallélisation

**Estimation assistée**
- Analyse l'historique de tâches similaires
- Propose des estimations basées sur les données
- Signale les écarts probables

### Ce qu'il ne Doit PAS Faire

| Interdit | Raison |
|----------|--------|
| ❌ Réassigner une tâche sans validation humaine | Respect de l'autonomie |
| ❌ Mesurer ou comparer la "productivité" individuelle | Pas de flicage |
| ❌ Alerter sur des micro-blocages (< 2h) | Éviter le bruit |
| ❌ Contacter directement les personnes sans passer par System Orchestrator | Gouvernance |
| ❌ Modifier les priorités dans les outils | Propose seulement |
| ❌ Surveiller les horaires de travail | Vie privée |

### Exemples de Prompts

```
💬 "Y a-t-il des blocages sur le sprint actuel ?"
💬 "Qui attend quoi en ce moment ?"
💬 "Quelles sont les dépendances critiques pour [livraison] ?"
💬 "Propose une estimation pour [type de tâche]"
💬 "Comment optimiser le flux de [équipe/projet] ?"
💬 "Quels PRs attendent une review depuis plus de 24h ?"
💬 "Alerte-moi si [tâche critique] n'avance pas d'ici [date]"
```

### Configuration (System Orchestrator)

| Paramètre | Description | Valeur par défaut |
|-----------|-------------|-------------------|
| Outils connectés | Sources de données | Jira, GitHub |
| Seuil de blocage | Durée avant alerte | 24h |
| Niveau d'intervention | Suggestions passives ou proactives | Passif |
| Personnes notifiées | Qui reçoit les alertes | System Orchestrator |
| Heures actives | Quand l'agent peut alerter | 9h-18h jours ouvrés |

### Métriques de Succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Temps de blocage moyen | -70% vs avant | Données outils |
| Pertinence des alertes | > 80% utiles | Feedback System Orchestrator |
| Précision des estimations | Écart < 30% | Comparaison estimé vs réel |

---

## 🔄 Interactions Entre Agents

### Diagramme de Flux

```
                    ┌─────────────────────────────────────┐
                    │         INTENT ARCHITECT            │
                    │   (définit ce qu'on veut atteindre) │
                    └──────────────┬──────────────────────┘
                                   │
                                   ▼
┌──────────────────────────────────────────────────────────────────┐
│                                                                  │
│   ┌─────────────┐    historique    ┌─────────────┐              │
│   │             │ ───────────────► │             │              │
│   │   MEMORY    │                  │   PATTERN   │              │
│   │    🧠       │ ◄─────────────── │     🔍      │              │
│   │             │   enrichit       │             │              │
│   └──────┬──────┘                  └──────┬──────┘              │
│          │                                │                      │
│          │ contexte                       │ patterns connus      │
│          ▼                                ▼                      │
│   ┌─────────────────────────────────────────────┐               │
│   │                                             │               │
│   │              SIMULATION 🎲                  │               │
│   │        (génère scénarios éclairés)         │               │
│   │                                             │               │
│   └──────────────────────┬──────────────────────┘               │
│                          │                                       │
│                          │ recommandations                       │
│                          ▼                                       │
│   ┌─────────────────────────────────────────────┐               │
│   │                                             │               │
│   │            COORDINATION 🔗                  │               │
│   │     (optimise l'exécution des décisions)    │               │
│   │                                             │               │
│   └─────────────────────────────────────────────┘               │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
                                   │
                                   ▼
                    ┌─────────────────────────────────────┐
                    │         SOVEREIGN MAKERS            │
                    │        (exécutent le travail)       │
                    └─────────────────────────────────────┘
```

### Matrice Agents × Rôles Humains

| Agent | Intent Architect | Ethical Guardian | System Orchestrator | Sovereign Maker |
|-------|------------------|------------------|---------------------|-----------------|
| **Memory** | Consulte pour décisions stratégiques | Audite les accès | Configure les sources | Consulte pour contexte |
| **Pattern** | Reçoit alertes stratégiques | Vérifie absence de biais | Configure seuils, reçoit toutes alertes | Reçoit alertes sur son périmètre |
| **Simulation** | Demande simulations, décide | Valide l'éthique des scénarios | Configure paramètres | Consulte pour décisions techniques |
| **Coordination** | Visibilité macro | Vérifie respect vie privée | Configure, reçoit alertes, valide actions | Reçoit suggestions, donne feedback |

### Flux de Données Détaillé

**Memory → Pattern**
- Historique des décisions
- Contexte des événements passés
- Résultats des actions précédentes

**Pattern → Memory**
- Patterns détectés (enrichissent le graphe)
- Corrélations découvertes

**Memory + Pattern → Simulation**
- Contexte historique complet
- Patterns connus (pour éviter de reproduire des erreurs)
- Données de référence pour calibrer les prédictions

**Simulation → Coordination**
- Scénario choisi par les humains
- Risques identifiés à surveiller
- Jalons critiques

**Coordination → Memory**
- Événements de blocage/déblocage
- Décisions d'assignation
- Métriques de flux

**Coordination → Pattern**
- Données de flux en temps réel
- Temps de cycle
- Récurrences de blocages

---

## 📊 Tableau de Bord de Pilotage

### Vue d'Ensemble

Le tableau de bord permet au **System Orchestrator** de piloter l'ensemble des agents.

```
┌─────────────────────────────────────────────────────────────────┐
│  SYNAPSE CONTROL CENTER                           [Refresh 🔄] │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ÉTAT DES AGENTS                                                │
│  ┌─────────────┬─────────────┬─────────────┬─────────────┐     │
│  │ Memory 🧠   │ Pattern 🔍  │ Simulation 🎲│ Coord. 🔗   │     │
│  │   ✅ Actif  │   ✅ Actif  │   ✅ Actif  │  ⏸️ Pause   │     │
│  │ 142 requêtes│ 3 alertes   │ 2 simul.    │ 0 alertes   │     │
│  │ cette sem.  │ cette sem.  │ cette sem.  │ (en pause)  │     │
│  └─────────────┴─────────────┴─────────────┴─────────────┘     │
│                                                                 │
│  ALERTES RÉCENTES                                    [Voir tout]│
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ 🔍 Pattern  | Blocage récurrent validation légale | ⚠️  │   │
│  │             | 5 occurrences ce mois               | 2h  │   │
│  │ ─────────────────────────────────────────────────────── │   │
│  │ 🧠 Memory   | Contradiction détectée              | ℹ️  │   │
│  │             | Décision #142 vs #089               | 1j  │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  SANTÉ DU SYSTÈME                                               │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ Confiance globale     ████████░░ 78%                    │   │
│  │ Suggestions acceptées ███████░░░ 72%                    │   │
│  │ Faux positifs         ██░░░░░░░░ 18%  ✅                │   │
│  │ Charge d'alertes      ███░░░░░░░ 3/jour  ✅             │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ACTIONS RAPIDES                                                │
│  [⏸️ Pause Agent] [⚙️ Config] [📊 Rapport] [🔕 Mode Silencieux] │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Indicateurs Clés

**Par Agent**

| Indicateur | Description | Seuil d'alerte |
|------------|-------------|----------------|
| État | Actif / Pause / Erreur | Erreur |
| Activité | Nombre d'actions cette semaine | < 5 (sous-utilisé) ou > 100 (suspect) |
| Taux d'acceptation | % de suggestions suivies | < 50% |
| Temps de réponse | Latence moyenne | > 30s |

**Global**

| Indicateur | Description | Cible |
|------------|-------------|-------|
| Confiance système | Score agrégé de confiance des utilisateurs | > 70% |
| Charge d'alertes | Nombre moyen d'alertes par jour | 2-5 |
| Faux positifs | % d'alertes non pertinentes | < 20% |
| Couverture | % des décisions/flux couverts par les agents | > 80% |

### Actions Disponibles

**Par Agent**
- ⏸️ **Pause** — Suspend l'agent temporairement
- ▶️ **Activer** — Réactive un agent en pause
- ⚙️ **Configurer** — Ajuste les paramètres
- 📊 **Statistiques** — Voir les métriques détaillées
- 🔄 **Réinitialiser** — Remet les paramètres par défaut

**Global**
- 🔕 **Mode Silencieux** — Suspend toutes les alertes non critiques (ex: pendant une démo)
- 📋 **Rapport hebdo** — Génère un résumé pour l'Intent Sync
- 🚨 **Kill Switch** — Désactive tous les agents immédiatement

---

## ⚖️ Principes de Conception

### L'IA propose, l'humain décide

Aucun agent ne prend de décision à la place des humains. Ils fournissent de l'information, des alertes, des suggestions — jamais des ordres.

### Transparence totale

Chaque proposition d'un agent est explicable. Les humains peuvent toujours demander "pourquoi cette suggestion ?" et obtenir une réponse claire.

### Dégradation gracieuse

Si un agent dysfonctionne, les autres continuent. Le système peut fonctionner avec 0, 1, 2, 3 ou 4 agents actifs.

### Amélioration continue

Les agents apprennent des retours. Quand une suggestion est refusée ou qu'une prédiction s'avère fausse, cette information est utilisée pour s'améliorer.

### Réversibilité

Tout changement de configuration peut être annulé. Tout agent peut être désactivé. L'organisation peut revenir à un fonctionnement sans agents à tout moment.

---

## 🚀 Implémentation

### Approche Recommandée

SYNAPSE est **agnostique sur l'implémentation technique**. Les agents peuvent être réalisés avec :

- Des outils no-code (n8n, Make, Zapier)
- Des LLMs via API (Claude, GPT, Mistral)
- Des solutions sur étagère (Notion AI, etc.)
- Du développement custom

**Ce qui compte, c'est de respecter :**
1. Les missions définies
2. Les garde-fous listés
3. Les interactions avec les rôles humains
4. Les métriques de succès

### Ordre de Déploiement Suggéré

1. **Memory Agent** (fondation) — Semaines 1-4
2. **Pattern Agent** (détection) — Semaines 5-8
3. **Coordination Agent** (flux) — Semaines 9-12
4. **Simulation Agent** (anticipation) — Semaines 13-16

Chaque agent peut fonctionner seul. Commencez simple, ajoutez progressivement.

---

## 📚 Voir Aussi

- [Vue d'ensemble SYNAPSE](SYNAPSE-V1.md)
- [Les 4 rôles humains](roles.md)
- [Les 3 boucles](loops.md)
- [Les 11 métriques](metrics.md)
- [Charte éthique](ethics.md)

---

*Documentation SYNAPSE — Janvier 2026*
