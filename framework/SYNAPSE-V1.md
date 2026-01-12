# SYNAPSE V1.0
## Framework de l'agilité cognitive

> **Architecture de co-évolution intelligente pour organisations hybrides (Humains + IA)**

---

## 🎯 VISION

SYNAPSE est un système d'organisation où l'intelligence est distribuée entre humains et agents IA, permettant une adaptation continue sans dépendre de rituels fixes ou de hiérarchies rigides.

**Ce que SYNAPSE n'est pas :**
- Un processus de gestion de projet
- Un remplacement des humains
- Un outil de surveillance
- Une nouvelle bureaucratie

**Ce que SYNAPSE est :**
- Un système cognitif distribué
- Une architecture socio-technique adaptative
- Un modèle de gouvernance hybride
- Une plateforme d'intelligence collective

---

## 🚀 État du Projet

### ✅ Composants Opérationnels (V1.0)

| Composant | Description | Statut |
|-----------|-------------|--------|
| **Memory Agent** | Mémoire organisationnelle, graphe de connaissances | ✅ Production |
| **Pattern Agent** | Détection de récurrences, alertes temps réel | ✅ Production |
| **Simulation Agent** | Scénarios probabilistes, aide à la décision | ✅ Production |
| **Coordination Agent** | Optimisation flux, détection blocages | ✅ Production |
| **Dashboard Métriques** | 11 métriques cognitives visualisées | ✅ Production |
| **Ethics Compliance** | Audits éthiques automatisés | ✅ Production |
| **Intent Hierarchy** | Organisation → Équipe | ✅ Production |
| **API Gateway** | TypeScript/Fastify/Prisma | ✅ Production |
| **Frontend** | React/Tailwind, i18n FR/EN | ✅ Production |

### 🔄 Prochaines Étapes

- Recherche d'organisations pilotes
- Validation terrain (2026)
- Publication académique
- SYNAPSE Cloud (option hébergée)

---

## 🏗️ ARCHITECTURE EN 3 COUCHES

```
┌─────────────────────────────────────────────────────────┐
│  COUCHE 1 : INTENTION (Humains)                         │
│  ↳ Définit le POURQUOI, le sens, les limites éthiques   │
│  ↳ Rôles : Intent Architect, Ethical Guardian           │
└─────────────────────────────────────────────────────────┘
                          ↓ Intention explicite
┌─────────────────────────────────────────────────────────┐
│  COUCHE 2 : COGNITION (IA + Humains)                    │
│  ↳ Modélise, mémorise, simule, détecte, propose         │
│  ↳ Agents : Memory, Pattern, Simulation, Coordination   │
└─────────────────────────────────────────────────────────┘
                          ↓ Options éclairées
┌─────────────────────────────────────────────────────────┐
│  COUCHE 3 : EXÉCUTION (Humains + IA)                    │
│  ↳ Matérialise dans le réel, ajuste, livre              │
│  ↳ Rôles : System Orchestrator, Sovereign Maker         │
└─────────────────────────────────────────────────────────┘
                          ↓ Feedback continu
                          ↑ (Boucle fermée)
```

**Principe clé** : Chaque couche informe la suivante. Le système apprend en continu.

---

## 👥 LES 4 RÔLES HUMAINS

### Intent Architect 🎯
Définit et maintient l'intention stratégique : objectifs, contraintes, limites éthiques.
**Pouvoir** : Veto si contraire à l'intention.

### Ethical Guardian ⚖️
Surveille les dérives éthiques, audite les décisions IA, protège les droits des personnes.
**Pouvoir** : Veto si dérive éthique.

### System Orchestrator 🎛️
Configure et optimise le système cognitif : active/désactive agents, définit règles, maintient infrastructure.
**Pouvoir** : Configuration du système.

### Sovereign Maker 🛠️
Matérialise les décisions dans le réel : code, produit, service.
**Pouvoir** : Accepte/refuse selon faisabilité.

👉 **[Descriptions complètes avec responsabilités, pouvoirs, exemples et antipatterns](roles.md)**

---

## 🤖 LES 4 AGENTS IA

| Agent | Mission | Statut |
|-------|---------|--------|
| **Memory Agent** 🧠 | Capture, structure et restitue la mémoire organisationnelle | ✅ Production |
| **Pattern Agent** 🔍 | Détecte les récurrences (blocages, inefficacités, opportunités) | ✅ Production |
| **Simulation Agent** 🎲 | Anticipe les conséquences de décisions (3-5 scénarios probabilistes) | ✅ Production |
| **Coordination Agent** 🔗 | Optimise les flux de travail et d'information | ✅ Production |

👉 **[Spécifications techniques complètes](agents.md)**

---

## 🔄 LES 3 BOUCLES

### Intent Sync 🎯 (Hebdomadaire, 30-45 min)
Vérifie l'alignement stratégique de l'organisation sur l'intention.
**Participants** : Tous les rôles.
**Output** : Intention validée ou ajustée + actions correctives.

### Pattern Review 🔍 (Continue + Hebdo, 15-30 min par pattern)
Examine les patterns détectés et décide des actions correctives.
**Participants** : Concernés par le pattern + System Orchestrator.
**Output** : Ignorer / Corriger / Expérimenter + plan d'action.

### Decision Moment ⚡ (À la demande, 30 min - 2h)
Prend une décision majeure éclairée par simulation et mémoire.
**Participants** : Décideurs + Simulation Agent.
**Output** : Décision formalisée + plan d'action + métriques suivi.

👉 **[Déroulements détaillés avec exemples concrets](loops.md)**

---

## 📊 LES 11 MÉTRIQUES COGNITIVES

**3 Catégories, 11 Métriques :**

### Métriques Système (5)
- Temps de cohérence
- Taux d'adaptation
- Mémoire active
- Clarté d'intention
- Latence de décision

### Métriques Humaines (3)
- Charge cognitive
- Autonomie perçue
- Confiance système

### Métriques de Valeur (3)
- Time to production
- Qualité livrée
- Coût d'adaptation

👉 **[Définitions précises, cibles et comment mesurer](metrics.md)**

---

## 🏗️ STACK TECHNIQUE V1

### Architecture

```
┌─────────────────────────────────────────────────┐
│                   Frontend                       │
│              React / Tailwind / i18n             │
└─────────────────────────────────────────────────┘
                        │
┌─────────────────────────────────────────────────┐
│               API Gateway                        │
│         TypeScript / Fastify / Prisma           │
└─────────────────────────────────────────────────┘
                        │
┌─────────────────────────────────────────────────┐
│                 Agents IA                        │
│   Memory │ Pattern │ Simulation │ Coordination  │
└─────────────────────────────────────────────────┘
                        │
┌─────────────────────────────────────────────────┐
│              Infrastructure                      │
│  PostgreSQL + pgvector │ Redis/Bull │ Ollama    │
└─────────────────────────────────────────────────┘
```

### Technologies

| Composant | Technologie | Rôle |
|-----------|-------------|------|
| API Gateway | TypeScript / Fastify | Routes, auth, validation |
| ORM | Prisma | Accès données typé, migrations |
| Base de données | PostgreSQL + pgvector | Données + recherche sémantique |
| Queue | Bull / Redis | Jobs asynchrones, scheduling |
| LLM Chat | 1min.ai / API externe | Raisonnement, génération |
| LLM Embeddings | Ollama (nomic-embed-text) | Vectorisation locale |
| Frontend | React / Tailwind | Interface utilisateur |
| Auth | JWT + API Keys | Sécurité |

### Déploiement

- **On-premise** : Fonctionne sur hardware minimal
- **Cloud privé** : Compatible toute infrastructure
- **Souveraineté** : Aucune dépendance cloud US obligatoire

---

## ⚖️ GOUVERNANCE ÉTHIQUE

**8 Principes non-négociables :**
1. Transparence algorithmique obligatoire
2. Droit de veto humain
3. Protection des données personnelles
4. Non-discrimination
5. Droit de contestation
6. Limitation de la surveillance
7. Consentement éclairé
8. Responsabilité humaine

**Charte des droits de l'employé :** Comprendre, contester, être protégé, déconnecter, apprendre, participer, refuser, auditer.

👉 **[Charte éthique complète + comité d'éthique](ethics.md)**

---

## 🚀 DÉMARRAGE

### Pour les organisations

**Phase 1 : Préparation** (2 semaines)
- Constituer les 4 rôles
- Rédiger l'Intent Statement
- Former l'équipe

**Phase 2 : Activation** (4-8 semaines)
- Déployer les agents progressivement
- Activer les 3 boucles
- Mesurer les métriques

**Phase 3 : Optimisation** (continue)
- Ajuster les configurations
- Traiter les patterns détectés
- Améliorer continuellement

👉 **[Guide d'implémentation détaillé](../docs/getting-started.md)**

---

## 🎯 CRITÈRES DE SUCCÈS

| Horizon | Validation |
|---------|-----------|
| **3 mois** | 4 rôles opérationnels, agents utilisés quotidiennement, premières décisions améliorées |
| **6 mois** | 3+ métriques dans le vert, -20% temps cycle, patterns traités régulièrement |
| **12 mois** | Système autonome, gains business mesurables, confiance système > 70% |

---

## 🌍 CONTRIBUTION

SYNAPSE est **open source** (CC BY-SA 4.0 pour la documentation).

**Contribuer :** Tester, améliorer, partager, documenter

👉 **[Guide de contribution](../CONTRIBUTING.md)**  
👉 **[Communauté](../community/README.md)**

---

## 📚 RESSOURCES

**Framework :**
- [Les 4 rôles humains](roles.md)
- [Les 4 agents IA](agents.md)
- [Les 3 boucles](loops.md)
- [Les 11 métriques](metrics.md)
- [Charte éthique](ethics.md)
- [Flux continu](continuous-flow.md)

**Guides pratiques :**
- [Guide d'implémentation](../docs/getting-started.md)
- [Templates](../templates/)
- [FAQ](../community/faq.md)
- [Glossaire](../docs/glossary.md)

---

## 🎬 CONCLUSION

SYNAPSE V1 est une plateforme complète et opérationnelle pour les organisations qui veulent dépasser l'agilité classique et co-évoluer avec l'IA.

**Les 4 agents sont opérationnels. Le framework est documenté. La stack est production-ready.**

Nous cherchons maintenant des organisations pilotes pour valider SYNAPSE en conditions réelles.

📧 Contact : synapse-origin@proton.me

---

*Document vivant - Dernière mise à jour : Janvier 2026*  
*Version : 1.0.0*
