# 📊 Les 11 Métriques Cognitives SYNAPSE

> **Source de vérité** pour tout ce qui concerne la mesure de performance d'une organisation hybride humains-IA.

---

## Vue d'Ensemble

SYNAPSE introduit **11 nouvelles métriques** pour mesurer la santé d'une organisation hybride. Ces métriques complètent (ne remplacent pas) les métriques agiles classiques.

### Les 3 Catégories

**Métriques Système (5)** : Santé du système hybride
- Temps de Cohérence
- Taux d'Adaptation
- Mémoire Active
- Clarté d'Intention
- Latence de Décision

**Métriques Humaines (3)** : Bien-être et efficacité
- Charge Cognitive
- Autonomie Perçue
- Confiance Système

**Métriques de Valeur (3)** : Impact business
- Temps de Mise en Production
- Qualité Livrée
- Coût d'Adaptation

---

## 📐 MÉTRIQUES SYSTÈME

### 1. Temps de Cohérence (Time to Coherence)

#### Définition
Délai entre une **décision** et son **intégration complète** dans le système : tous les acteurs (humains et agents) sont alignés et agissent en conséquence.

#### Pourquoi C'est Important
Dans une organisation distribuée (humains + IA), une décision ne suffit pas. Il faut que l'information se propage, que les agents se reconfigurent, que les humains ajustent leurs actions.

#### Comment Mesurer

**Formule :**
```
Temps de Cohérence = Timestamp Alignement Complet - Timestamp Décision
```

**Étapes :**
1. **T0** : Décision formalisée (enregistrée dans Memory Agent)
2. **T1** : Tous les agents IA mis à jour
3. **T2** : Tous les humains concernés informés
4. **T3** : Premières actions conformes observées
5. **T4** : Aucune action contradictoire pendant 24h

**Temps de Cohérence = T4 - T0**

#### Cibles Recommandées

| Type de Décision | Cible | Acceptable | Problématique |
|------------------|-------|------------|---------------|
| Opérationnelle | < 24h | < 48h | > 72h |
| Tactique | < 3 jours | < 1 semaine | > 2 semaines |
| Stratégique | < 1 semaine | < 2 semaines | > 1 mois |

#### Exemple
```
Décision (Lundi 10h) : "Feature X est priorité absolue"

T0+2h : Memory Agent enregistre
T0+4h : Intent Sync → tous les rôles informés
T0+1 jour : Première PR sur Feature X
T0+2 jours : Aucune action sur autre feature

Temps de Cohérence = 2 jours ✅
```

---

### 2. Taux d'Adaptation (Adaptation Rate)

#### Définition
Pourcentage de **patterns détectés** qui mènent à une **action concrète** implémentée.

#### Pourquoi C'est Important
Détecter des patterns ne sert à rien si on n'agit pas. Cette métrique mesure si l'organisation **apprend et s'adapte** réellement.

#### Comment Mesurer

**Formule :**
```
Taux d'Adaptation = (Actions Implémentées / Patterns Détectés) × 100
```

#### Cibles Recommandées

| Contexte | Cible | Interprétation |
|----------|-------|----------------|
| Startup agile | > 60% | Organisation réactive |
| Scale-up | > 50% | Bon équilibre |
| Grande entreprise | > 40% | Acceptable |

**Attention :**
- Trop bas (< 30%) : Patterns ignorés
- Trop haut (> 80%) : Peut-être trop de faux positifs

#### Exemple
```
Novembre : 15 patterns détectés
- 5 négatifs → 4 traités (80%)
- 8 neutres → 0 traités (normal)
- 2 positifs → 2 généralisés (100%)

Taux d'Adaptation = 6/15 = 40% ✅
```

---

### 3. Mémoire Active (Active Memory Rate)

#### Définition
Pourcentage de **décisions** qui réutilisent des **connaissances historiques** plutôt que de les redécouvrir.

#### Pourquoi C'est Important
Une organisation sans mémoire répète les mêmes erreurs. Memory Agent est efficace si cette métrique est élevée.

#### Comment Mesurer

**Formule :**
```
Mémoire Active = (Décisions Informées par Historique / Total Décisions) × 100
```

**Critères "informée" :**
- Memory Agent a fourni contexte pertinent
- Contexte consulté par le décideur
- Décideur confirme que ça a influencé sa décision

#### Cibles Recommandées

| Phase | Cible | Interprétation |
|-------|-------|----------------|
| Mois 1-3 | > 20% | Memory se constitue |
| Mois 4-6 | > 30% | Mémoire utile |
| Mois 7+ | > 40% | Mémoire active |

**Plafond réaliste : 50-60%**

#### Exemple
```
Semaine : 12 décisions
Informées par historique : 5

Mémoire Active = 5/12 = 42% ✅
```

---

### 4. Clarté d'Intention (Intent Clarity Score)

#### Définition
Degré de **consensus et compréhension partagée** sur les objectifs stratégiques.

#### Pourquoi C'est Important
Si les gens ne comprennent pas l'intention, chacun tire dans une direction différente.

#### Comment Mesurer

**Questionnaire hebdomadaire (échelle 1-10) :**
```
1. "Je comprends l'objectif principal"
2. "Je connais nos 3 priorités stratégiques"
3. "Je sais si mes décisions alignent avec l'intention"
4. "Les autres rôles et moi sommes d'accord sur où on va"
5. "L'Intent Statement est clair et actionnable"

Score = Moyenne
```

#### Cibles Recommandées

| Score | Interprétation | Action |
|-------|----------------|--------|
| > 8/10 | Excellent | Maintenir |
| 6-8/10 | Bon | Clarifier points |
| 4-6/10 | Confusion | Intent Sync extra |
| < 4/10 | Critique | Réécrire Intent |

#### Exemple
```
15 répondants :
Q1: 8.2, Q2: 6.5⚠️, Q3: 7.8, Q4: 7.1, Q5: 6.9

Score global : 7.3/10 ✅

Action : Q2 faible → clarifier priorités
```

---

### 5. Latence de Décision (Decision Latency)

#### Définition
Temps entre l'**identification d'un besoin de décision** et la **décision effective**.

#### Pourquoi C'est Important
La vitesse de décision est un avantage compétitif. SYNAPSE doit accélérer grâce à simulation et mémoire.

#### Comment Mesurer

**Formule :**
```
Latence = Timestamp Décision - Timestamp Besoin
```

#### Cibles Recommandées

| Type | Cible | Acceptable | Trop Lent |
|------|-------|------------|-----------|
| Opérationnelle | < 4h | < 24h | > 48h |
| Tactique | < 48h | < 1 sem | > 2 sem |
| Stratégique | < 1 sem | < 2 sem | > 1 mois |

#### Exemple
```
"Embaucher un DevOps ?"

T0 (Lundi 9h) : Besoin mentionné
T4 (Mardi 11h) : Décision formalisée

Latence = 26h ✅

Sans SYNAPSE : 3-4 semaines
→ SYNAPSE a divisé par ~10
```

---

## 👤 MÉTRIQUES HUMAINES

### 6. Charge Cognitive (Cognitive Load)

#### Définition
Niveau de **sollicitation mentale** ressenti par les humains.

#### Pourquoi C'est Important
L'IA doit **soulager** la charge cognitive, pas la **surcharger**.

#### Comment Mesurer

**Questionnaire hebdomadaire (1-10) :**
```
"Cette semaine, votre charge mentale ?"

1-3 : Faible (ennui)
4-6 : Optimale (flow)
7-8 : Élevée (gérable)
9-10 : Excessive (surcharge)
```

#### Cibles Recommandées

| Score | Interprétation | Action |
|-------|----------------|--------|
| 4-6 | Optimal | Maintenir |
| 6-7 | Élevé acceptable | Surveiller |
| 7-8 | Préoccupant | Réduire sollicitations |
| > 8 | Critique | Intervention |

#### Exemple
```
8 personnes, Semaine 47 :
Moyenne : 6.3/10 ✅

David à 8/10 ⚠️ → Investigation
Cause : Incident technique (exceptionnel)
```

---

### 7. Autonomie Perçue (Perceived Autonomy)

#### Définition
Sentiment de **contrôler ses décisions** malgré les propositions IA.

#### Pourquoi C'est Important
Si les humains se sentent "pilotés" par l'IA, c'est un échec.

#### Comment Mesurer

**Questionnaire mensuel (1-10) :**
```
1. "Je contrôle mes décisions"
2. "L'IA propose, je décide librement"
3. "Je peux refuser l'IA sans justification"
4. "Je suis plus autonome qu'avant SYNAPSE"
5. "L'IA m'aide, elle ne décide pas"

Score = Moyenne
```

#### Cibles Recommandées

| Score | Interprétation | Action |
|-------|----------------|--------|
| > 8/10 | Excellent | Maintenir |
| 7-8/10 | Bon | Continuer |
| 5-7/10 | Préoccupant | Ajuster balance |
| < 5/10 | Critique | Revoir gouvernance |

#### Exemple
```
12 répondants :
Score : 8.0/10 ✅ Excellent

Commentaire : "Je décide mieux, plus vite. L'IA me booste."
```

---

### 8. Confiance Système (System Trust)

#### Définition
Degré de **confiance** dans les propositions IA.

#### Pourquoi C'est Important
Sans confiance, les humains ignorent l'IA ou la suivent aveuglément (dangereux).

#### Comment Mesurer

**Taux d'acceptation :**
```
Confiance = (Propositions Acceptées / Total) × 100
```

#### Cibles Recommandées

| Score | Interprétation | Action |
|-------|----------------|--------|
| 70-80% | Optimal | Confiance calibrée |
| 60-70% | Acceptable | Améliorer précision |
| 50-60% | Bas | Revoir qualité |
| < 50% | Critique | Système ignoré |
| > 90% | Suspect | Compliance aveugle ? |

#### Exemple
```
42 propositions IA :
- Memory : 13/15 acceptées (87%)
- Pattern : 11/18 acceptées (61%)
- Simulation : 7/9 acceptées (78%)

Confiance = 74% ✅ Optimal
```

---

## 💼 MÉTRIQUES DE VALEUR

### 9. Temps de Mise en Production

#### Définition
Délai entre l'**idée initiale** et le **déploiement en production**.

#### Pourquoi C'est Important
SYNAPSE doit accélérer grâce à mémoire, simulation, coordination.

#### Comment Mesurer

**Formule :**
```
Time to Production = Date Déploiement - Date Idée
```

#### Cibles Recommandées

| Feature | Avant SYNAPSE | Avec SYNAPSE | Amélioration |
|---------|---------------|--------------|--------------|
| Petite | 5-7 jours | 3-4 jours | -40% |
| Moyenne | 15-20 jours | 10-12 jours | -40% |
| Grande | 2-3 mois | 1.5-2 mois | -30% |

#### Exemple
```
Feature "Export CSV" :

Sans SYNAPSE : 19 jours
Avec SYNAPSE : 9 jours (Memory réutilise code passé)

Gain : -53% ✅
```

---

### 10. Qualité Livrée

#### Définition
Taux de **bugs/incidents** en production après déploiement.

#### Pourquoi C'est Important
La vitesse ne doit pas sacrifier la qualité.

#### Comment Mesurer

**Formule :**
```
Qualité = (Bugs Production / Features Déployées) × 100
```

#### Cibles Recommandées

| Métrique | Cible | Action si Dépassé |
|----------|-------|-------------------|
| Bugs critiques | < 2% | Investigation |
| Bugs mineurs | < 10% | Acceptable |
| Hotfixes | < 5% | Revoir tests |

#### Exemple
```
Mois : 20 features déployées
- 1 bug critique (5%) ⚠️
- 3 bugs mineurs (15%)
- 1 hotfix (5%)

Action : Investiguer cause du bug critique
```

---

### 11. Coût d'Adaptation

#### Définition
Effort nécessaire pour **changer de direction** stratégique.

#### Pourquoi C'est Important
SYNAPSE doit faciliter les pivots.

#### Comment Mesurer

**Méthode :**
Comparer effort changement avant/après SYNAPSE
```
Coût = Temps + Ressources pour pivoter
```

#### Cibles Recommandées

| Changement | Avant | Avec SYNAPSE | Amélioration |
|------------|-------|--------------|--------------|
| Pivot mineur | 2 sem | 1 sem | -50% |
| Pivot majeur | 2 mois | 1 mois | -50% |

#### Exemple
```
Pivot : B2C → B2B

Sans SYNAPSE : 8 semaines
Avec SYNAPSE : 4 semaines
- Simulation accélère décision (2 sem → 2 jours)
- Memory évite redécouverte (réutilise patterns B2B passés)
- Coordination optimise réallocation équipe

Gain : -50% ✅
```

---

## 📊 Dashboard Recommandé

### Vue d'Ensemble

```
┌─────────────────────────────────────────┐
│ SYNAPSE HEALTH DASHBOARD                │
├─────────────────────────────────────────┤
│ SYSTÈME                    │ HUMAINS     │
│ Cohérence    : 2j    ✅   │ Charge : 6/10 ✅│
│ Adaptation   : 65%   ✅   │ Autonomie : 8/10 ✅│
│ Mémoire      : 42%   ✅   │ Confiance : 74% ✅│
│ Intention    : 7.3/10 ✅  │              │
│ Latence      : 26h   ✅   │              │
├─────────────────────────────────────────┤
│ VALEUR                                   │
│ Time to Prod : -40%  ✅                  │
│ Qualité      : 5% bugs ⚠️                │
│ Adapt. Cost  : -50%  ✅                  │
└─────────────────────────────────────────┘
```

### Alertes Automatiques

**Seuils d'alerte :**
- 🔴 Critique : Intervention immédiate
- 🟡 Attention : Surveiller
- 🟢 OK : RAS

---

## 📈 Évolution dans le Temps

### Tracking Mensuel

```
Mois 1-3 : Installation
- Établir baseline
- Commencer mesure
- Accepter que certaines métriques soient basses

Mois 4-6 : Stabilisation
- Métriques commencent à s'améliorer
- Identifier patterns
- Ajuster système

Mois 7-12 : Maturité
- Métriques cibles atteintes
- Système autonome
- Amélioration continue
```

---

## 🎯 Priorisation des Métriques

### Phase de Démarrage (Mois 1-3)
**Focus sur :**
1. Clarté d'Intention (fondation)
2. Charge Cognitive (bien-être)
3. Confiance Système (adoption)

### Phase de Croissance (Mois 4-6)
**Ajouter :**
4. Mémoire Active
5. Taux d'Adaptation
6. Temps de Cohérence

### Phase de Maturité (Mois 7+)
**Mesurer tout :**
- Les 11 métriques
- Comparaisons avant/après
- Benchmark avec autres organisations

---

## 📚 Voir Aussi

**Framework SYNAPSE :**
- [Vue d'ensemble complète](SYNAPSE-V0.1.md)
- [Les 4 Rôles Humains](roles.md)
- [Les 4 Agents IA](agents.md)
- [Les 3 Boucles](loops.md)

**Guides Pratiques :**
- [Guide d'implémentation](../docs/getting-started.md)
- [Templates](../templates/)
- [FAQ](../community/faq.md)

---

*Source de vérité maintenue par la communauté SYNAPSE*  
*Dernière mise à jour : Novembre 2025*
