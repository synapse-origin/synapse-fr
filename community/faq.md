# ❓ Questions Fréquentes (FAQ)

---

## Général

### Qu'est-ce que SYNAPSE exactement ?

SYNAPSE est un framework d'organisation où humains et intelligences artificielles collaborent dans une relation symbiotique. Ce n'est pas un outil, mais une nouvelle façon de structurer et faire fonctionner une organisation.

### Quel est l'état actuel du projet ?

**SYNAPSE V1.0 est opérationnel** (Janvier 2026) :
- ✅ 4 agents IA en production (Memory, Pattern, Simulation, Coordination)
- ✅ Dashboard avec 11 métriques cognitives
- ✅ Ethics Compliance System
- ✅ API Gateway TypeScript/Fastify
- ✅ Frontend React complet

Nous recherchons maintenant des **organisations pilotes** pour valider le framework en conditions réelles.

### En quoi c'est différent de l'agilité (Scrum, Kanban, SAFe) ?

| Aspect | Agilité Classique | SYNAPSE |
|--------|------------------|---------|
| Décisions | Humains seuls | Humains + IA |
| Adaptation | Cycles fixes (sprints) | Continue (temps réel) |
| Mémoire | Documentation manuelle | Graphe de connaissances auto-généré |
| Coordination | Rituels humains (daily, retro) | Détection automatique + intervention ciblée |
| Patterns | Détectés en rétro (trop tard) | Temps réel |

SYNAPSE ne complète pas l'agilité, il la remplace.

---

## Technique

### Quelles technologies sont utilisées ?

**Stack V1 :**

| Composant | Technologie |
|-----------|-------------|
| API Gateway | TypeScript / Fastify |
| ORM | Prisma |
| Base de données | PostgreSQL + pgvector |
| Queue | Bull / Redis |
| LLM Chat | 1min.ai ou API externe |
| LLM Embeddings | Ollama (local) |
| Frontend | React / Tailwind |

### Combien ça coûte ?

**Option cloud/API :**
- Infrastructure : 50-100€/mois
- APIs LLM : 50-200€/mois
- **Total : ~100-300€/mois**

**Option souveraine (tout local) :**
- Hardware one-time : ~500€
- LLM : Ollama gratuit
- **Coût récurrent : ~0€**

### Peut-on déployer entièrement en local ?

**Oui !** C'est même un des différenciateurs de SYNAPSE :
- PostgreSQL + pgvector : local
- Ollama : LLM local (Mistral, Llama, etc.)
- Aucune dépendance cloud obligatoire
- 100% souveraineté des données

### Comment gérez-vous la sécurité des données ?

**Principes :**
- Chiffrement at-rest et in-transit
- Authentification JWT + API Keys
- RBAC (Role-Based Access Control)
- Logs d'audit complets
- Déploiement on-premise possible

**RGPD :**
- Droit à l'oubli implémenté
- Minimisation des données
- Transparence totale

---

## Organisationnel

### Mon équipe est résistante au changement. Comment convaincre ?

**Stratégie :**
1. **Commencer petit** : 1 équipe volontaire
2. **Montrer, ne pas dire** : Résultats concrets > promesses
3. **Impliquer tôt** : Co-construire, pas imposer
4. **Célébrer les victoires** : Communiquer chaque amélioration

**Argument clé :** L'IA aide, ne remplace pas. Les humains restent aux commandes.

### Combien de temps avant de voir des résultats ?

**1 mois :** Memory Agent réduit le temps de recherche d'info

**3 mois :** Patterns détectés et traités, décisions de meilleure qualité

**6-12 mois :** Transformation profonde, gains business mesurables

### Quels types d'organisations peuvent utiliser SYNAPSE ?

**Idéal pour :**
- Équipes tech / produit (5-50 personnes)
- Startups / scale-ups en croissance
- Départements innovation

**Moins adapté pour :**
- Organisations très réglementées sans marge de manœuvre
- Contextes où l'expérimentation est impossible

### Que se passe-t-il si un agent IA se trompe ?

**Garde-fous en place :**
1. Les humains décident toujours (l'IA propose)
2. Ethical Guardian audite en continu
3. Alertes automatiques sur anomalies
4. Traçabilité complète
5. Possibilité de désactiver un agent

---

## Éthique

### L'IA ne va-t-elle pas remplacer les humains ?

**Non.** SYNAPSE **augmente** les capacités humaines :

**Ce que l'IA fait mieux :**
- Mémoire parfaite
- Détection de patterns
- Calculs et simulations

**Ce que les humains gardent :**
- Définir le sens et l'intention
- Jugement éthique
- Créativité
- Décisions en incertitude radicale

### Comment évitez-vous les biais algorithmiques ?

**Mesures V1 :**
1. Ethical Guardian comme rôle dédié
2. Audits éthiques automatisés (8 principes)
3. Score de conformité visible
4. Alertes si dérive détectée
5. Droit de contestation

### Qu'est-ce qui empêche la surveillance des employés ?

**Garde-fous éthiques :**
1. Charte des droits intégrée
2. Interdictions explicites (keylogging, scoring individuel...)
3. Transparence : chacun sait ce qui est capturé
4. Ethical Guardian avec pouvoir de veto

---

## Adoption

### Par où commencer ?

1. **Lire** : [SYNAPSE V1](../framework/SYNAPSE-V1.md) (30 min)
2. **Comprendre** : Les 4 rôles, 4 agents, 3 boucles
3. **Expérimenter** : [Guide d'implémentation](../docs/getting-started.md)
4. **Rejoindre** : [Discussions GitHub](https://github.com/synapse-origin/synapse-fr/discussions)

### Faut-il abandonner Scrum/Kanban pour utiliser SYNAPSE ?

**Transition progressive possible :**

**Phase 1 (Hybride) :**
- Gardez vos sprints
- Ajoutez Memory Agent
- Observez

**Phase 2 (Transition) :**
- Réduisez certains rituels
- Augmentez l'autonomie des agents
- Les boucles SYNAPSE remplacent certaines cérémonies

**Phase 3 (SYNAPSE pur) :**
- Adaptation continue
- Plus de cycles fixes

### Comment devenir organisation pilote ?

**Critères :**
- Équipe tech/produit (5-50 personnes)
- Volontaires pour expérimenter (3-6 mois)
- Capacité à documenter et partager

**Process :**
1. Contact : synapse-origin@proton.me
2. Échange de qualification
3. Onboarding personnalisé

**En échange :**
- Support direct
- Accès prioritaire aux évolutions
- Co-construction du framework

---

## Comparaison

### SYNAPSE vs SAFe ?

| Aspect | SAFe | SYNAPSE |
|--------|------|---------|
| Philosophie | Process-driven | Intelligence-driven |
| Coordination | Hiérarchie + rituels | Agents IA + humains |
| Adaptation | Cycles trimestriels | Continue |
| IA | Absente | Au cœur |

### SYNAPSE vs Holacracy ?

| Aspect | Holacracy | SYNAPSE |
|--------|-----------|---------|
| Philosophie | Auto-gouvernance pure | Hybridation humain-IA |
| Rôles | Fluides, nombreux | 4 rôles fixes + agents |
| IA | Absente | Centrale |

---

## Support

### J'ai un problème, où demander de l'aide ?

1. **Documentation** : [/docs](../docs/)
2. **FAQ** : Vous y êtes !
3. **Discussions** : [GitHub](https://github.com/synapse-origin/synapse-fr/discussions)
4. **Email** : synapse-origin@proton.me

### Je veux contribuer, comment faire ?

- [Guide de contribution](../CONTRIBUTING.md)
- Documentation et templates ouverts
- Traductions bienvenues
- Études de cas recherchées

---

**Votre question n'est pas ici ?**

👉 [Ouvrez une discussion GitHub](https://github.com/synapse-origin/synapse-fr/discussions)

---

*FAQ SYNAPSE V1*  
*Dernière mise à jour : Janvier 2026*
