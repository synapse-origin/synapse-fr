# 👥 Les 4 Rôles Humains dans SYNAPSE

> **Source de vérité** pour tout ce qui concerne les rôles humains dans SYNAPSE.

---

## Vue d'Ensemble

SYNAPSE définit **4 rôles humains essentiels** qui collaborent avec les agents IA pour créer une organisation hybride adaptative.

| Rôle | Focus | Pouvoir Principal | Interaction IA |
|------|-------|-------------------|----------------|
| **Intent Architect** | Stratégie & Sens | Veto si contraire à l'intention | Définit objectifs pour les agents |
| **Ethical Guardian** | Éthique & Intégrité | Veto si dérive éthique | Audite les décisions IA |
| **System Orchestrator** | Configuration Système | Active/désactive agents | Configure les agents |
| **Sovereign Maker** | Matérialisation | Décide de la faisabilité | Co-crée avec agents |

---

## 🎯 Intent Architect (Architecte d'Intention)

### Mission
Définir et maintenir la cohérence stratégique de l'organisation : le **pourquoi** nous existons, **où** nous allons, et **ce qui ne peut être compromis**.

### Responsabilités

**Définition Stratégique :**
- Formaliser l'Intent Statement (objectifs, contraintes, hors scope)
- Expliciter les objectifs en langage clair et mesurable
- Définir les contraintes non-négociables (légales, éthiques, business)
- Clarifier ce qui est hors scope

**Maintien de la Cohérence :**
- Valider que les actions du système servent l'intention
- Arbitrer les conflits entre objectifs contradictoires
- Détecter et corriger les dérives stratégiques
- Adapter l'intention si le contexte change fondamentalement

**Alignement Organisationnel :**
- Animer l'Intent Sync hebdomadaire
- S'assurer que tous les rôles comprennent l'intention
- Communiquer les changements stratégiques

### Pouvoirs de Décision

**VETO sur :**
- Toute décision contraire à l'intention déclarée
- Toute action qui compromet les contraintes non-négociables
- Tout pivot stratégique non justifié

**Redéfinition de :**
- Objectifs stratégiques (si contexte change)
- Priorisation des intentions (en cas de conflit)
- Périmètre de l'organisation (scope)

### Interactions avec les Agents IA

**Inputs vers IA :**
- Alimente le système avec Intent Statements formalisés
- Définit les critères de succès mesurables
- Communique les changements de priorité

**Outputs de l'IA :**
- Reçoit alertes si dérive détectée (Memory Agent)
- Obtient simulations d'impact de changements stratégiques (Simulation Agent)
- Consulte historique des intentions passées (Memory Agent)

### Métriques de Performance

| Métrique | Cible | Comment Mesurer |
|----------|-------|-----------------|
| Clarté d'intention | > 80% | Questionnaire hebdomadaire tous rôles |
| Temps de convergence après changement | < 1 semaine | Timestamp changement → alignement complet |
| Taux de décisions alignées | > 90% | Décisions conformes / Total décisions |
| Satisfaction stratégique équipe | > 7/10 | Questionnaire mensuel |

### Profil Idéal

**Compétences Essentielles :**
- Vision stratégique à moyen/long terme
- Capacité de formalisation et synthèse
- Aisance avec l'ambiguïté et l'incertitude
- Communication claire et inspirante

**Pas Nécessaire :**
- Compétences techniques poussées
- Expertise IA/ML
- Background développement

**Qualités Personnelles :**
- Assertivité (capacité à dire non)
- Patience (construire consensus prend du temps)
- Humilité (accepter de se tromper)
- Courage (défendre l'intention face aux pressions)

### Exemples Concrets

**Situation 1 : Détection de Dérive**
```
Contexte: L'équipe se disperse sur 10 features différentes

Intent Architect observe:
- Intent Statement dit "Focus sur PME manufacturières"
- 7/10 features en cours concernent le retail
- Aucune feature PME manufacturières depuis 2 mois

Action:
1. Convoque Intent Sync extraordinaire
2. Rappelle l'intention
3. Décide: 5 features retail stoppées, ressources réallouées
4. Met à jour Intent Statement si le retail devient stratégique
```

**Situation 2 : Arbitrage de Conflit**
```
Conflit: 
- Objectif A: "Croissance rapide" (+50 clients en 3 mois)
- Objectif B: "Qualité irréprochable" (0 bugs critiques)
- Ces 2 objectifs sont en tension

Intent Architect:
1. Consulte Simulation Agent (impact de chaque scénario)
2. Décide: "Qualité prime. Croissance +20 clients suffit."
3. Justification: "Notre différenciation = qualité, pas volume"
4. Communique à toute l'équipe
```

### Antipatterns (À Éviter)

❌ **Micromanagement** : L'Intent Architect ne décide pas des détails d'implémentation  
❌ **Changement permanent** : Changer l'intention toutes les semaines = chaos  
❌ **Intention vague** : "Être le meilleur" n'est pas une intention exploitable  
❌ **Déconnexion terrain** : Rester dans l'abstraction sans écouter les makers  
❌ **Veto systématique** : User du veto trop souvent = perte de crédibilité

---

## ⚖️ Ethical Guardian (Gardien Éthique)

### Mission
Protéger l'**intégrité humaine et éthique** du système. Garantir que l'optimisation algorithmique ne se fasse jamais au détriment des valeurs, des droits des personnes, ou de l'éthique.

### Responsabilités

**Surveillance Continue :**
- Auditer les décisions IA pour détecter biais et dérives
- Analyser les patterns suspects (discrimination, suroptimisation)
- Vérifier la transparence algorithmique
- Suivre les métriques d'équité

**Protection des Personnes :**
- Garantir les droits des personnes impactées par le système
- Traiter les contestations de décisions IA
- Assurer la conformité RGPD
- Protéger la vie privée

**Gouvernance Éthique :**
- Maintenir et faire évoluer la charte éthique
- Animer le comité d'éthique (si existant)
- Former l'organisation à l'éthique de l'IA
- Gérer les incidents éthiques

### Pouvoirs de Décision

**VETO sur :**
- Toute décision éthiquement problématique
- Toute fonctionnalité IA qui viole la charte éthique
- Tout traitement de données contraire au RGPD
- Toute décision discriminatoire (prouvée)

**Suspension de :**
- Agent IA en cas de comportement anormal
- Fonctionnalité IA jusqu'à correction
- Processus automatisé si risque avéré

### Interactions avec les Agents IA

**Outputs de l'IA :**
- Accès total aux logs de décision des agents
- Dashboard d'audit en temps réel
- Alertes automatiques sur patterns suspects

### Métriques de Performance

| Métrique | Cible | Comment Mesurer |
|----------|-------|-----------------|
| Dérives éthiques détectées et corrigées | 100% détectées | Audits surprise + tests adverses |
| Temps de réponse aux alertes | < 48h | Timestamp alerte → action |
| Score de confiance système | > 70% | Questionnaire mensuel équipe |
| Conformité RGPD | 100% | Audits externes annuels |

### Profil Idéal

**Compétences Essentielles :**
- Compréhension des biais IA et fairness
- Connaissances en protection des données (RGPD)
- Capacité d'analyse critique
- Indépendance d'esprit

**Qualités Personnelles :**
- Courage (dire non à la hiérarchie si nécessaire)
- Intégrité (résister aux compromis éthiques)
- Empathie (comprendre impact sur les personnes)
- Rigueur (documenter, tracer, auditer)

### Exemples Concrets

**Situation 1 : Biais Détecté**
```
Alerte: Pattern Agent détecte que les "feedbacks négatifs" 
        sont 2x plus fréquents pour un groupe démographique

Ethical Guardian:
1. Analyse approfondie (40 décisions récentes)
2. Confirme: biais dans l'interprétation des feedbacks
3. Identifie cause: données d'entraînement biaisées
4. Action immédiate: 
   - Suspend fonctionnalité feedback automatique
   - Réentraînement avec données équilibrées
   - Tests de fairness avant réactivation
5. Documentation: rapport public + apprentissages
```

**Situation 2 : Demande de Surveillance Invasive**
```
Direction demande: "On veut tracker la productivité 
                    individuelle minute par minute"

Ethical Guardian:
1. Consulte charte éthique (interdit explicitement)
2. Évalue alternatives (métriques agrégées d'équipe OK)
3. Répond: VETO sur tracking individuel
4. Propose: Dashboard d'équipe anonymisé
5. Justification: Protection vie privée + charte signée
```

---

## 🎛️ System Orchestrator (Orchestrateur Système)

### Mission
Configurer et optimiser le **système cognitif** SYNAPSE : activer/désactiver agents, définir règles d'interaction, maintenir l'infrastructure technique, assurer performance et fiabilité.

### Responsabilités

**Configuration du Système :**
- Activer/désactiver les agents IA selon besoins
- Définir les règles d'interaction entre agents
- Paramétrer les seuils d'alerte et de détection
- Configurer les intégrations (Git, Slack, etc.)

**Optimisation des Flux :**
- Optimiser les flux d'information entre humains et agents
- Identifier et résoudre les goulots d'étranglement
- Réduire la latence du système
- Améliorer la pertinence des propositions IA

**Maintenance Technique :**
- Assurer la disponibilité du système (uptime)
- Gérer les mises à jour et déploiements
- Monitorer les performances et coûts
- Résoudre les incidents techniques

### Pouvoirs de Décision

**Configuration des Agents :**
- Fréquence d'exécution (temps réel, horaire, quotidienne)
- Priorités et poids des différents agents
- Règles de déclenchement des alertes
- Niveau d'autonomie accordé à chaque agent

**Interventions Système :**
- Redémarrage d'un agent si dysfonctionnel
- Modification de configuration en production
- Rollback si nouvelle config problématique

### Métriques de Performance

| Métrique | Cible | Comment Mesurer |
|----------|-------|-----------------|
| Uptime du système | > 99% | Monitoring continu |
| Temps de réponse système | < 5s (90e percentile) | Logs de performance |
| Taux de résolution incidents | < 4h (incidents critiques) | Tickets incidents |
| Satisfaction technique équipe | > 7/10 | Questionnaire mensuel |

### Profil Idéal

**Compétences Essentielles :**
- Architecture systèmes distribués
- Compréhension technique des systèmes IA/ML
- DevOps / SRE (reliability engineering)
- Monitoring et observabilité

**Qualités Personnelles :**
- Vision systémique (voir les interdépendances)
- Pragmatisme (équilibre entre idéal et réalité)
- Rigueur (documenter, tester avant prod)
- Curiosité (tester nouvelles approches)

### Exemples Concrets

**Situation 1 : Optimisation de Latence**
```
Problème: Pattern Agent prend 15s pour répondre (trop lent)

System Orchestrator:
1. Analyse les logs (goulot: recherche dans Memory Agent)
2. Identifie solution: cache Redis pour requêtes fréquentes
3. Implémente cache en staging
4. Teste (latence réduite à 2s)
5. Déploie en production
6. Monitor résultats
```

---

## 🛠️ Sovereign Maker (Créateur Souverain)

### Mission
Matérialiser les décisions dans le **réel tangible** : écrire le code, designer le produit, livrer le service. Le Maker travaille en symbiose avec les agents IA mais garde le contrôle créatif et la responsabilité du résultat.

### Responsabilités

**Matérialisation :**
- Transformer les décisions en réalité (code, design, contenu)
- Choisir les technologies et architectures
- Implémenter les features décidées
- Livrer en production

**Arbitrage Qualité :**
- Décider des compromis qualité/vitesse/coût
- Garantir la viabilité technique des décisions
- Maintenir la dette technique sous contrôle
- Refuser une demande si techniquement infaisable

**Collaboration IA :**
- Utiliser les agents IA comme assistants (pair programming, code review)
- Alimenter le Memory Agent avec difficultés d'implémentation
- Challenger les propositions IA si irréalistes

### Pouvoirs de Décision

**Acceptation/Refus :**
- Accepter ou refuser les propositions du système si infaisables
- Demander re-simulation si hypothèses techniques fausses
- Proposer solutions alternatives

**Choix Techniques :**
- Technologies utilisées
- Architectures et patterns
- Outils et frameworks

### Métriques de Performance

| Métrique | Cible | Comment Mesurer |
|----------|-------|-----------------|
| Temps décision → implémentation | < 2 jours | Timestamps |
| Taux de propositions IA implémentables | > 70% | Acceptées / Total |
| Qualité du résultat | < 5% bugs en production | Incidents post-deploy |
| Dette technique | < 20% de la codebase | Analyse statique |

### Profil Idéal

**Compétences Essentielles :**
- Expertise métier (dev, design, ops selon contexte)
- Capacité d'exécution rapide et qualitative
- Pragmatisme (équilibre idéal vs réalité)

**Qualités Personnelles :**
- Sens du résultat (livrer, pas juste concevoir)
- Adaptabilité (ajuster si plan change)
- Humilité (accepter suggestions IA)
- Créativité (trouver solutions originales)

### Exemples Concrets

**Situation 1 : Proposition IA Infaisable**
```
Simulation Agent propose: "Migrer vers microservices en 2 semaines"

Sovereign Maker:
1. Évalue la faisabilité (IMPOSSIBLE en 2 semaines)
2. Explique au système: "Migration complète = 3-4 mois minimum"
3. Propose alternative: "Migration progressive, 1 service par mois"
4. Demande nouvelle simulation avec hypothèses réalistes
5. Accepte la proposition ajustée
```

---

## 🔗 Interactions Entre Rôles

### Matrice de Collaboration

| De → Vers | Intent Architect | Ethical Guardian | System Orchestrator | Sovereign Maker |
|-----------|------------------|------------------|---------------------|-----------------|
| **Intent Architect** | - | Valide éthique intention | Demande config agents | Communique priorités |
| **Ethical Guardian** | Alerte dérives | - | Demande audits système | Revoit décisions |
| **System Orchestrator** | Propose optimisations | Fournit logs audit | - | Optimise outils |
| **Sovereign Maker** | Remonte infaisabilités | Signale risques éthiques | Demande features tech | - |

---

## 📊 Tableau Récapitulatif

| Dimension | Intent Architect | Ethical Guardian | System Orchestrator | Sovereign Maker |
|-----------|------------------|------------------|---------------------|-----------------|
| **Focus** | Stratégie | Éthique | Système | Exécution |
| **Horizon** | 6-12 mois | Continu | Temps réel | Semaines |
| **Type décision** | Quoi & Pourquoi | Peut-on ? | Comment optimiser ? | Concrètement |
| **Pouvoir principal** | Veto stratégique | Veto éthique | Configuration | Acceptation/Refus |
| **Compétence clé** | Vision | Intégrité | Technique | Expertise métier |
| **% Temps** | 20-30% | 20-30% | 30-40% | 60-80% |

---

## 📚 Voir Aussi

**Framework SYNAPSE :**
- [Vue d'ensemble complète](SYNAPSE-V0.1.md)
- [Les 4 Agents IA](agents.md)
- [Les 3 Boucles](loops.md)
- [Charte Éthique](ethics.md)

**Guides Pratiques :**
- [Guide d'implémentation](../docs/getting-started.md)
- [Templates](../templates/)
- [FAQ](../community/faq.md)

---

*Source de vérité maintenue par la communauté SYNAPSE*  
*Dernière mise à jour : Novembre 2025*
