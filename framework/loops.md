# 🔄 Les 3 boucles SYNAPSE

> **Source de vérité** pour tout ce qui concerne les boucles (rituels) dans SYNAPSE.

---

## Vue d'ensemble

SYNAPSE remplace les **rituels agiles classiques** (daily standup, sprint planning, retrospective) par **3 boucles de feedback** optimisées pour une organisation hybride humains-IA.

| Boucle | Objectif | Fréquence | Durée | Participants Clés |
|--------|----------|-----------|-------|-------------------|
| **Intent Sync** | Alignement stratégique | Hebdomadaire | 30-45 min | Tous les rôles |
| **Pattern Review** | Traiter les récurrences | Continue + Hebdo | 15-30 min | Concernés + System Orchestrator |
| **Decision Moment** | Décisions majeures | À la demande | 30 min - 2h | Décideurs + Simulation Agent |

**Principe fondamental** : Les boucles s'adaptent aux besoins, pas l'inverse.

---

## 🎯 Intent sync (Synchronisation d'intention)

### Objectif
Vérifier que l'organisation **reste alignée** sur l'intention stratégique. Détecter et corriger les dérives avant qu'elles ne deviennent problématiques.

### Fréquence & timing
- **Standard** : Hebdomadaire (ex: tous les lundis 10h)
- **Ajustable** : Bi-hebdomadaire si organisation stable
- **Extraordinaire** : Sur demande si changement majeur

### Déclencheurs

**Automatique :**
- Date/heure prévue

**Sur Alerte :**
- Memory Agent détecte contradiction majeure
- Pattern Agent signale dérive systématique
- Intent Architect convoque session extraordinaire

**Sur événement :**
- Changement stratégique de l'organisation
- Pivot produit
- Crise externe (marché, réglementation)

### Participants

**Obligatoires :**
- Intent Architect (anime)
- Ethical Guardian
- System Orchestrator
- Sovereign Maker(s)

**Optionnels :**
- Stakeholders externes (clients, investisseurs)
- Représentants d'équipes élargies

### Déroulement (45 min)

**1. Rappel de l'intention (5 min)**
```
Intent Architect présente :
- Intent Statement actuel
- Objectifs stratégiques
- Contraintes non-négociables
```

**2. Revue des décisions récentes (10 min)**
```
Memory agent présente :
- 10-15 décisions majeures de la semaine
- Leur alignement avec l'intention (score)
- Contradictions détectées

Exemple:
"Décision #142 : 'Développer feature X'
 Alignement : 85% avec Objectif Stratégique #2
 ⚠️ Contradiction mineure avec Contrainte #1"
```

**3. Détection de dérives (10 min)**
```
Pattern Agent présente :
- Patterns de dérive détectés
- Métriques d'alignement sur 4 semaines
- Tendances préoccupantes

Exemple:
"⚠️ Dérive détectée : 
 Les 8 dernières décisions priorisent court terme 
 vs notre intention 'Vision long terme'"
```

**4. Discussion & décisions (15 min)**
```
Tous les rôles débattent :
- L'intention est-elle toujours valide ?
- Faut-il la clarifier/ajuster ?
- Quelles actions correctives ?

Décisions possibles :
→ Maintenir l'intention (aucun changement)
→ Clarifier l'intention (reformulation)
→ Ajuster l'intention (contexte a changé)
→ Actions correctives (réaligner décisions)
```

**5. Actions & suivi (5 min)**
```
Intent Architect formalise :
- Décisions prises
- Actions assignées (qui fait quoi)
- Métriques de suivi
- Prochaine revue
```

### Outputs

**Documentés :**
- Intent Statement (mis à jour si modifié)
- Actions correctives assignées
- Décisions de réalignement
- Log dans Memory Agent

**Communiqués :**
- Synthèse envoyée à toute l'organisation
- Changements majeurs annoncés publiquement
- Mise à jour des dashboards

### Métriques de succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Clarté post-Intent Sync | > 80% | Questionnaire après session |
| Actions correctives implémentées | > 90% | Suivi à J+7 |
| Temps de convergence | < 1 semaine | Alignement complet mesuré |
| Participation active | > 80% présents | Attendance + engagement |

### Exemples concrets

**Session normale (Pas de dérive)**
```
Memory Agent: "15 décisions cette semaine, alignement moyen 92%"
Pattern Agent: "Aucune dérive systématique détectée"
Intent Architect: "OK, on continue. Prochaine revue lundi prochain."
Durée: 30 min
```

**Session avec dérive détectée**
```
Pattern Agent: "⚠️ 7/10 décisions concernent feature X, 
                mais notre intention prioritaire = feature Y"

Discussion:
- Pourquoi ce glissement ? (Feature X demandée par gros client)
- Est-ce un problème ? (Oui, on s'éloigne de notre cœur de métier)
- Action : Finir feature X en cours, puis 100% focus sur feature Y

Intent Architect: Met à jour priorités, communique à l'équipe
Durée: 50 min
```

### Antipatterns

❌ **Rubber-stamp** : Valider automatiquement sans vraie discussion  
❌ **Micro-management** : Descendre dans détails d'implémentation  
❌ **Débat infini** : Philosopher sans décider  
❌ **Absence de suivi** : Décider des actions mais ne pas les implémenter  
❌ **Exclusion** : Ne pas inclure tous les rôles concernés

---

## 🔍 Pattern Review (Revue des patterns)

### Objectif
Examiner les **patterns récurrents** détectés par Pattern Agent et décider des **actions correctives** ou **expérimentations** pour les traiter.

### Fréquence & timing

**Continue (Alertes temps réel) :**
- Pattern Agent envoie alertes si pattern significatif détecté
- Traitement immédiat si critique

**Hebdomadaire (Revue systématique) :**
- Tous les vendredis 14h (exemple)
- Revue de tous les patterns de la semaine

### Déclencheurs

**Alertes automatiques :**
- Seuil d'occurrence franchi (ex: blocage répété 3 fois)
- Dégradation de métrique (ex: vélocité -20%)
- Pattern positif intéressant (bonne pratique émergente)

**Revue systématique :**
- Date/heure prévue
- Même si aucun pattern critique (prévention)

### Participants

**Obligatoires :**
- System Orchestrator (anime)
- Personnes concernées par le pattern

**Selon contexte :**
- Ethical Guardian (si implications éthiques)
- Intent Architect (si impact stratégique)
- Sovereign Maker(s) (si solution technique nécessaire)

### Déroulement (30 min)

**1. Présentation du pattern (5 min)**
```
Pattern Agent présente :
- Type de pattern (blocage, inefficacité, opportunité)
- Données chiffrées (fréquence, impact)
- Personnes/équipes impactées
- Historique (première vs dernière occurrence)

Exemple:
"📊 PATTERN #47 : Blocage Validation Légale
 - Fréquence : 8 occurrences en 2 mois
 - Impact moyen : +3 jours de délai par feature
 - Personnes : ÉquipeA, ServiceLégal
 - Coût estimé : 24 jours perdus (€24k)"
```

**2. Analyse des causes (10 min)**
```
Discussion collective :
- Pourquoi ce pattern existe ?
- Quelles sont les causes racines ?
- Est-ce un problème ou un symptôme ?

Techniques :
- 5 Whys
- Fishbone diagram (si complexe)
- Revue de décisions passées (Memory Agent)
```

**3. Décision sur action (10 min)**
```
Options possibles :

A) IGNORER
- Pattern pas significatif finalement
- Coût correction > bénéfice
- Documenter pourquoi on ignore

B) CORRIGER
- Action corrective immédiate
- Changer un processus / règle
- Former les personnes

C) EXPÉRIMENTER
- Lancer une expérimentation
- Mesurer l'impact pendant N semaines
- Décider ensuite de généraliser

D) ESCALADER
- Pattern trop complexe pour Pattern Review
- Nécessite Intent Sync ou Decision Moment
```

**4. Plan d'action (5 min)**
```
Si décision B ou C :
- Qui fait quoi ?
- Quand ?
- Comment on mesure le succès ?
- Suivi à quelle date ?
```

### Outputs

**Documentés :**
- Pattern analysé (description, causes)
- Décision prise (ignorer/corriger/expérimenter)
- Actions assignées
- Métriques de suivi
- Log dans Memory Agent

**Communiqués :**
- Synthèse aux personnes impactées
- Mise à jour des règles système (si changement)
- Dashboard patterns mis à jour

### Métriques de succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Taux d'adaptation | > 60% | Actions / Patterns détectés |
| Impact mesurable corrections | > 80% patterns améliorés | Métriques avant/après |
| Taux de faux positifs | < 20% | Patterns ignorés / Total |
| Délai traitement patterns critiques | < 48h | Timestamp alerte → action |

### Exemples concrets

**Pattern négatif : Blocage récurrent**
```
Pattern: "Toujours bloqué sur validation légale"

Analyse:
- Cause racine : Service légal contacté trop tard
- 60% des cas : documentation manquante

Action: CORRIGER
1. Nouveau process : Légal impliqué dès conception
2. Template documentation légale créé
3. Formation équipe sur requis légaux
4. Mesure dans 1 mois : délai validation légale

Résultat (1 mois après) :
- Délai validation : 5 jours → 1.5 jours (-70%)
- Documentation complète : 40% → 95%
```

**Pattern positif : Bonne pratique émergente**
```
Pattern: "Pair programming sur bugs critiques = -40% temps résolution"

Analyse:
- 5 bugs critiques résolus en pair programming
- Temps moyen : 2h vs 5h en solo
- Taux de régression : -60%

Action: GÉNÉRALISER
1. Recommander pair programming pour tous bugs critiques
2. Ajouter dans guidelines équipe
3. Mesurer adoption et impact

Résultat :
- Pratique adoptée par 80% de l'équipe
- Temps résolution bugs critiques : -35% global
```

### Antipatterns

❌ **Analysis paralysis** : Analyser à l'infini sans décider  
❌ **Solution systématique** : Créer une règle lourde pour chaque pattern  
❌ **Ignorer patterns positifs** : Focus uniquement sur problèmes  
❌ **Pas de suivi** : Décider actions mais ne jamais vérifier l'impact  
❌ **Blame game** : Chercher un coupable au lieu de comprendre le système

---

## ⚡ Decision Moment (Moment de décision)

### Objectif
Prendre une **décision importante** de façon éclairée en s'appuyant sur les **simulations** du Simulation Agent et la **mémoire** organisationnelle.

### Fréquence & timing
- **À la demande** : Pas de fréquence fixe
- **Déclenchement** : Quand une décision complexe/majeure doit être prise

### Déclencheurs

**Par un Rôle :**
- Intent Architect : Décision stratégique
- Sovereign Maker : Choix technique majeur
- Ethical Guardian : Dilemme éthique

**Par le système :**
- Simulation Agent détecte opportunité
- Pattern Agent identifie besoin de décision
- Memory Agent rappelle décision similaire passée

### Participants

**Toujours :**
- Rôle concerné par la décision (décideur final)
- Simulation Agent (présente scénarios)

**Selon contexte :**
- Autres rôles si décision transverse
- Experts (techniques, métier, externes)
- Stakeholders impactés

### Déroulement (Variable : 30 min - 2h)

**1. Formulation de la décision (10 min)**
```
Décideur formule clairement :
- Quelle décision doit être prise ?
- Pourquoi maintenant ?
- Quelles contraintes ?
- Quel horizon temporel ?

Exemple:
"Décision : Faut-il migrer vers architecture microservices ?
 Pourquoi : Scalabilité actuelle insuffisante
 Contraintes : Budget 150k€, équipe de 5 devs
 Horizon : Décision pour les 12 prochains mois"
```

**2. Contexte historique (10 min)**
```
Memory Agent fournit :
- Décisions similaires passées
- Leurs résultats (succès/échec)
- Leçons apprises
- Contexte qui a changé depuis

Exemple:
"Il y a 2 ans, décision similaire (Decision #089)
 Option choisie : Rester monolithe
 Raison : 'Simplicité'
 Résultat : Positif pendant 18 mois, maintenant limites atteintes
 Contexte changé : x10 utilisateurs, nouvelles exigences"
```

**3. Simulation de scénarios (20-30 min)**
```
Simulation Agent présente 3-5 scénarios :

SCÉNARIO A : Migration complète (6 mois)
- Probabilité succès : 60%
- Coût : 180k€
- Bénéfices : +40% scalabilité, -80% downtime
- Risques : Migration BDD complexe, tests e2e
- Timeline : [Gantt détaillé]

SCÉNARIO B : Migration progressive (12 mois)
- Probabilité succès : 80%
- Coût : 240k€
- Bénéfices : +30% scalabilité, risques distribués
- Risques : Dette technique hybride
- Timeline : [Gantt détaillé]

RECOMMANDATION IA (confiance 70%) : SCÉNARIO B
Raison : Meilleur équilibre risque/bénéfice
```

**4. Discussion & délibération (20-40 min)**
```
Débat collectif :
- Quel scénario aligné avec intention ?
- Quels risques acceptables ?
- Que faire si ça se passe mal ?
- Y a-t-il alternatives non explorées ?

Techniques :
- Pre-mortem : "Imaginez qu'on a échoué. Pourquoi ?"
- Devil's advocate : Défendre scénario contraire
- Simulation ajustée si hypothèses changent
```

**5. Décision formalisée (10 min)**
```
Décideur tranche :
- Scénario choisi : [X]
- Justification : [Pourquoi]
- Plan d'action : [Qui fait quoi, quand]
- Métriques de suivi : [Comment mesurer succès]
- Révision prévue : [Date]

Enregistré dans Memory Agent
```

**6. Suivi & apprentissage (Post-décision)**
```
À M+1, M+3, M+6 :
- Comparer prédictions vs réalité
- Analyser les écarts
- Améliorer les modèles de simulation
- Documenter les apprentissages
```

### Outputs

**Documentés :**
- Decision Record complet
- Scénarios simulés
- Décision prise + justification
- Plan d'action détaillé
- Métriques de suivi
- Log dans Memory Agent

### Métriques de succès

| Métrique | Cible | Mesure |
|----------|-------|--------|
| Latence de décision | < 48h pour décisions majeures | Timestamp besoin → décision |
| Précision des prédictions | Écart < 20% | Prédiction vs réalité à M+3 |
| Satisfaction des décideurs | > 7/10 | Questionnaire post-Decision Moment |
| Taux d'implémentation | > 90% | Décisions effectivement appliquées |

### Exemples concrets

**Décision technique simple**
```
Décision : "Quel framework frontend ?"

Simulation Agent :
- React : Familier équipe, 5 jours
- Vue : Plus simple, 4 jours mais courbe apprentissage
- Angular : Overkill pour cette feature

Décision : React (familiarité > gain 1 jour)
Durée : 30 min
```

**Décision stratégique complexe**
```
Décision : "Pivoter vers B2B vs rester B2C ?"

Simulation Agent : 4 scénarios détaillés
Memory Agent : 3 pivots similaires dans historique
Discussion : 1h30 (tous les rôles)

Décision : Pivot B2B progressif (test 6 mois)
Justification : Meilleure unit economics
Suivi : Revue à M+3

Durée : 2h
```

### Antipatterns

❌ **Décision hâtive** : Trancher sans simulation ni contexte  
❌ **Analysis paralysis** : Demander 10 scénarios sans jamais décider  
❌ **Ignorer la simulation** : Décider selon intuition seule  
❌ **Pas de suivi** : Ne jamais vérifier si prédictions étaient justes  
❌ **Décision solitaire** : Décider seul sans consulter

---

## 🔄 Comparaison avec rituels agile

| Aspect | Agile Classique | SYNAPSE |
|--------|----------------|---------|
| **Planning** | Sprint Planning (2-4h/2 sem) | Intent Sync (45 min/sem) |
| **Coordination** | Daily Standup (15 min/jour) | Coordination Agent + alertes |
| **Adaptation** | Retrospective (1-2h/2 sem) | Pattern Review (continu) |
| **Décision** | Consensus ou PO | Simulation + Rôle décide |
| **Fréquence** | Cycles fixes | Adaptative |

**Gains SYNAPSE :**
- ✅ Moins de temps en réunions (-40%)
- ✅ Feedback plus rapide (continu vs fin de sprint)
- ✅ Décisions éclairées (simulation vs intuition)
- ✅ Mémoire organisationnelle (vs documentation ad-hoc)

---

## 🎯 Quand utiliser quelle boucle ?

### Intent Sync
**Utilisez pour :**
- ✅ Vérifier alignement stratégique
- ✅ Détecter dérives
- ✅ Ajuster l'intention si contexte change

**N'utilisez PAS pour :**
- ❌ Décisions opérationnelles détaillées
- ❌ Résolution de bugs
- ❌ Planning de tâches

### Pattern Review
**Utilisez pour :**
- ✅ Traiter récurrences
- ✅ Capitaliser sur bonnes pratiques
- ✅ Optimiser processus

**N'utilisez PAS pour :**
- ❌ Incidents ponctuels
- ❌ Décisions stratégiques majeures
- ❌ Résolution immédiate

### Decision Moment
**Utilisez pour :**
- ✅ Décisions majeures
- ✅ Choix avec multiples options complexes
- ✅ Besoin de simulation

**N'utilisez PAS pour :**
- ❌ Décisions triviales
- ❌ Urgences (pas le temps)
- ❌ Décisions déjà alignées

---

## 📚 Voir Aussi

**Framework SYNAPSE :**
- [Vue d'ensemble complète](SYNAPSE-V0.1.md)
- [Les 4 rôles humains](roles.md)
- [Les 4 agents IA](agents.md)
- [Métriques cognitives](metrics.md)

**Guides pratiques :**
- [Guide d'implémentation](../docs/getting-started.md)
- [Templates](../templates/)
- [FAQ](../community/faq.md)

---

*Source de vérité maintenue par la communauté SYNAPSE*  
*Dernière mise à jour : Novembre 2025*
