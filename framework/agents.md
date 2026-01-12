# 🤖 Les 4 agents IA dans SYNAPSE

> **Tous les agents sont opérationnels en V1.0**

Les agents IA de SYNAPSE ne remplacent pas les humains. Ils **augmentent** leur capacité à comprendre, décider et agir dans un système complexe.

---

## Vue d'ensemble

| Agent | Fonction | Statut | Déclenchement |
|-------|----------|--------|---------------|
| **Memory Agent** 🧠 | Mémoire organisationnelle | ✅ Production | Continu (passif) |
| **Pattern Agent** 🔍 | Détection de récurrences | ✅ Production | Continu (actif) + alertes |
| **Simulation Agent** 🎲 | Anticipation | ✅ Production | À la demande |
| **Coordination Agent** 🔗 | Optimisation des flux | ✅ Production | Continu + proactif |

---

## 🧠 Memory Agent

### Mission
Être la **mémoire parfaite** de l'organisation. Capturer, structurer et restituer toute la connaissance collective.

### Statut : ✅ Production

### Capacités Implémentées

#### 1. Capture automatique
- Décisions formalisées via API
- Extraction d'entités par LLM
- Génération d'embeddings pour recherche sémantique
- Stockage dans graphe de connaissances

#### 2. Recherche contextuelle
- Recherche sémantique (pgvector)
- Récupération de contexte pertinent
- Suggestions basées sur l'historique

#### 3. Détection de contradictions
- Analyse des nouvelles décisions vs historique
- Alertes si incohérence détectée
- Traçabilité complète

### Stack Technique

```typescript
// Architecture Memory Agent
{
  "api": "Fastify + TypeScript",
  "orm": "Prisma",
  "database": "PostgreSQL + pgvector",
  "llm_chat": "1min.ai API",
  "llm_embeddings": "Ollama (nomic-embed-text)",
  "queue": "Bull / Redis"
}
```

### Endpoints Principaux

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/decisions` | POST | Créer une décision |
| `/api/decisions/search` | POST | Recherche sémantique |
| `/api/decisions/:id/context` | GET | Contexte historique |
| `/api/memory/contradictions` | GET | Contradictions détectées |

---

## 🔍 Pattern Agent

### Mission
Identifier les **récurrences** (bonnes ou mauvaises) dans le comportement de l'organisation.

### Statut : ✅ Production

### Capacités Implémentées

#### 1. Détection de patterns négatifs
- Blocages récurrents
- Goulots d'étranglement
- Dépassements systématiques

#### 2. Détection de patterns positifs
- Bonnes pratiques émergentes
- Configurations efficaces
- Succès reproductibles

#### 3. Système d'alertes
- Alertes temps réel si seuil franchi
- Notifications configurables
- Historique des alertes

#### 4. Jobs planifiés
- Analyse périodique (toutes les 6h)
- Consolidation hebdomadaire
- Rapports automatiques

### Stack Technique

```typescript
// Architecture Pattern Agent
{
  "scheduler": "Bull / Redis",
  "analysis": "Prisma queries + LLM",
  "alerts": "Event-driven",
  "storage": "PostgreSQL"
}
```

### Endpoints Principaux

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/patterns` | GET | Liste des patterns |
| `/api/patterns/detect` | POST | Lancer détection |
| `/api/patterns/:id/actions` | POST | Enregistrer action |
| `/api/alerts` | GET | Alertes actives |

---

## 🎲 Simulation Agent

### Mission
**Anticiper** les conséquences de décisions avant de les prendre. Transformer l'incertitude en scénarios quantifiés.

### Statut : ✅ Production

### Capacités Implémentées

#### 1. Génération de scénarios
- 3-5 scénarios par décision
- Probabilités de succès estimées
- Risques identifiés par scénario

#### 2. Analyse contextuelle
- Intégration avec Memory Agent
- Prise en compte de l'historique
- Apprentissage des décisions passées

#### 3. Recommandations
- Scénario recommandé avec justification
- Niveau de confiance
- Alternatives proposées

### Stack Technique

```typescript
// Architecture Simulation Agent
{
  "llm": "1min.ai API (claude/gpt)",
  "context": "Memory Agent integration",
  "output": "Structured JSON scenarios",
  "storage": "PostgreSQL"
}
```

### Endpoints Principaux

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/simulations` | POST | Créer simulation |
| `/api/simulations/:id` | GET | Détails simulation |
| `/api/simulations/:id/scenarios` | GET | Scénarios générés |
| `/api/decisions/:id/simulate` | POST | Simuler une décision |

### Exemple de Sortie

```json
{
  "decision": "Migrer vers microservices",
  "scenarios": [
    {
      "name": "Migration complète (6 mois)",
      "probability": 0.60,
      "benefits": ["Scalabilité +40%", "Résilience améliorée"],
      "risks": ["Complexité migration BDD", "Courbe apprentissage"],
      "cost": "180k€",
      "timeline": "6 mois"
    },
    {
      "name": "Migration progressive (12 mois)",
      "probability": 0.80,
      "benefits": ["Risques distribués", "Apprentissage continu"],
      "risks": ["Dette technique hybride", "Durée projet"],
      "cost": "240k€",
      "timeline": "12 mois"
    }
  ],
  "recommendation": {
    "scenario": "Migration progressive",
    "confidence": 0.75,
    "rationale": "Meilleur équilibre risque/bénéfice"
  }
}
```

---

## 🔗 Coordination Agent

### Mission
Optimiser les **flux** de travail et d'information. Identifier les dépendances, anticiper les blocages, suggérer des interventions.

### Statut : ✅ Production

### Capacités Implémentées

#### 1. Détection de blocages
- Analyse des tâches en attente
- Identification des dépendances bloquantes
- Alertes proactives

#### 2. Suggestions d'intervention
- Réassignation proposée
- Priorisation suggérée
- Optimisation des flux

#### 3. Analyse des dépendances
- Graphe de dépendances
- Chemin critique identifié
- Goulots détectés

### Stack Technique

```typescript
// Architecture Coordination Agent
{
  "analysis": "Prisma + custom algorithms",
  "scheduler": "Bull / Redis",
  "notifications": "Event-driven",
  "storage": "PostgreSQL"
}
```

### Endpoints Principaux

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/coordination/blockers` | GET | Blocages détectés |
| `/api/coordination/suggestions` | GET | Suggestions actives |
| `/api/coordination/dependencies` | GET | Graphe dépendances |
| `/api/coordination/optimize` | POST | Lancer optimisation |

---

## 🔄 Intent Sync (Consolidation)

### Mission
Consolider hebdomadairement l'alignement entre les décisions et l'intention stratégique.

### Statut : ✅ Production

### Capacités Implémentées

- Score d'alignement calculé automatiquement
- Identification des dérives
- Rapport consolidé hebdomadaire
- Historique des Intent Syncs

### Endpoints

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/intent-sync` | POST | Lancer consolidation |
| `/api/intent-sync/history` | GET | Historique |
| `/api/intent-sync/:id` | GET | Détails d'un sync |

---

## 📊 Dashboard & Métriques

### Statut : ✅ Production

### 11 Métriques Cognitives Implémentées

**Système (5):**
- Temps de cohérence
- Taux d'adaptation
- Mémoire active
- Clarté d'intention
- Latence de décision

**Humaines (3):**
- Charge cognitive
- Autonomie perçue
- Confiance système

**Valeur (3):**
- Time to production
- Qualité livrée
- Coût d'adaptation

### Endpoints

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/metrics/cognitive` | GET | Toutes les métriques |
| `/api/metrics/dashboard` | GET | Vue dashboard |
| `/api/metrics/history` | GET | Historique |

---

## ⚖️ Ethics Compliance

### Statut : ✅ Production

### Capacités Implémentées

- Audits éthiques automatisés
- Score de conformité par principe
- Alertes si dérive détectée
- Historique des audits

### 8 Principes Audités

1. Transparence algorithmique
2. Droit de veto humain
3. Protection des données
4. Non-discrimination
5. Droit de contestation
6. Limitation surveillance
7. Consentement éclairé
8. Responsabilité humaine

### Endpoints

| Endpoint | Méthode | Description |
|----------|---------|-------------|
| `/api/ethics/audit` | POST | Lancer audit |
| `/api/ethics/score` | GET | Score actuel |
| `/api/ethics/history` | GET | Historique audits |

---

## 🏗️ Architecture Globale

```
┌─────────────────────────────────────────────────────────┐
│                      Frontend React                      │
│                   (Dashboard, Forms, i18n)               │
└─────────────────────────────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────┐
│                 API Gateway (Fastify)                    │
│              Auth (JWT/API Keys) + Validation            │
└─────────────────────────────────────────────────────────┘
                            │
        ┌───────────────────┼───────────────────┐
        ▼                   ▼                   ▼
┌───────────────┐   ┌───────────────┐   ┌───────────────┐
│ Memory Agent  │   │ Pattern Agent │   │  Simulation   │
│               │   │               │   │    Agent      │
└───────────────┘   └───────────────┘   └───────────────┘
        │                   │                   │
        └───────────────────┼───────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────┐
│              Coordination Agent                          │
│         (Orchestration, Blockers, Suggestions)           │
└─────────────────────────────────────────────────────────┘
                            │
        ┌───────────────────┼───────────────────┐
        ▼                   ▼                   ▼
┌───────────────┐   ┌───────────────┐   ┌───────────────┐
│  PostgreSQL   │   │  Redis/Bull   │   │    Ollama     │
│  + pgvector   │   │   (Queue)     │   │  (Embeddings) │
└───────────────┘   └───────────────┘   └───────────────┘
```

---

## 🔐 Sécurité

### Authentification
- JWT pour sessions utilisateur
- API Keys pour intégrations
- RBAC (Role-Based Access Control)

### Protection des données
- Chiffrement at-rest (PostgreSQL)
- HTTPS obligatoire
- Logs d'audit complets

---

## 📈 Métriques de Performance

| Métrique | Cible | Actuel |
|----------|-------|--------|
| Latence API | < 200ms | ✅ |
| Uptime | > 99% | ✅ |
| Temps génération simulation | < 30s | ✅ |
| Précision recherche sémantique | > 80% | ✅ |

---

## 🚀 Déploiement

### Prérequis
- Node.js 18+
- PostgreSQL 15+ avec pgvector
- Redis 7+
- Ollama (pour embeddings locaux)

### Variables d'environnement

```env
DATABASE_URL=postgresql://...
REDIS_URL=redis://...
ONEMIN_API_KEY=...
JWT_SECRET=...
OLLAMA_URL=http://localhost:11434
```

### Commandes

```bash
# Installation
npm install

# Migrations
npx prisma migrate deploy

# Démarrage
npm run start
```

---

## 📚 Voir Aussi

- [Vue d'ensemble SYNAPSE V1](SYNAPSE-V1.md)
- [Les 4 rôles humains](roles.md)
- [Les 3 boucles](loops.md)
- [Les 11 métriques](metrics.md)
- [Charte éthique](ethics.md)

---

*Agents SYNAPSE V1.0 - Tous opérationnels*  
*Dernière mise à jour : Janvier 2026*
