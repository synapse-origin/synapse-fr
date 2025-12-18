# ❓ Questions Fréquentes (FAQ)

---

## Général

### Qu'est-ce que SYNAPSE exactement ?

SYNAPSE est un framework d'organisation où humains et intelligences artificielles collaborent dans une relation symbiotique. Ce n'est pas un outil, mais une nouvelle façon de structurer et faire fonctionner une organisation.

### En quoi c'est différent de l'agilité (Scrum, Kanban, SAFe) ?

| Aspect | Agilité Classique | SYNAPSE |
|--------|------------------|---------|
| Décisions | Humains seuls | Humains + IA |
| Adaptation | Cycles fixes (sprints) | Continue (temps réel) |
| Mémoire | Documentation manuelle | Graphe de connaissances auto-généré |
| Coordination | Rituels humains (daily, retro) | Détection automatique + intervention ciblée |

SYNAPSE ne remplace pas l'agilité, il la fait évoluer pour l'ère de l'IA.

### Pourquoi créer un nouveau framework ?

L'agilité a 24 ans. Elle a fonctionné, mais montre ses limites :
- Rituels devenus des fins en soi
- Coordination humaine saturée au-delà de 50 personnes
- Cycles trop lents face à la complexité actuelle
- L'IA existe maintenant et peut transformer la façon de travailler

SYNAPSE intègre l'IA dès la conception, pas comme un add-on.

---

## Technique

### Quelles technologies sont utilisées ?

**Agents IA :**
- LLMs : GPT-4, Claude (raisonnement)
- Vector databases : Pinecone, Weaviate (mémoire sémantique)
- Graph databases : Neo4j (relations et connaissances)
- Time series : InfluxDB (métriques)

**Infrastructure :**
- Backend : Python (FastAPI) ou Node.js
- Frontend : React/Next.js
- Orchestration : Docker, Kubernetes
- Event streaming : Kafka, RabbitMQ

Tout est modulaire et remplaçable.

### Combien ça coûte ?

**Phase pilote (1 équipe, 3 mois) :**
- Infrastructure cloud : 200-500€/mois
- APIs IA (OpenAI/Anthropic) : 100-300€/mois
- Outils divers : 100€/mois
- **Total** : ~400-900€/mois

**À échelle (50+ personnes) :**
- ~2000-5000€/mois selon usage

**Alternative low-cost :**
- LLMs open source (Llama, Mistral) : auto-hébergés
- Coût réduit à l'infrastructure seule (~500€/mois)

### Est-ce que je peux utiliser des LLMs open source ?

Oui ! SYNAPSE est agnostique sur les technologies :
- Llama 3, Mistral, etc. peuvent remplacer GPT-4
- Vector databases open source (Qdrant, Chroma)
- Tout peut être auto-hébergé

Trade-off : performance des LLMs commerciaux > open source (pour l'instant).

### Quelles intégrations sont disponibles ?

**Actuellement (V0.1) :**
- Git (GitHub, GitLab)
- Communication (Slack, Teams)
- Project Management (API générique)

**Roadmap Q1 2026 :**
- Jira, Linear, Asana
- Notion, Confluence
- Datadog, Grafana

### Comment gérez-vous la sécurité des données ?

**Principes :**
- Chiffrement at-rest et in-transit
- Accès basé sur rôles (RBAC)
- Logs d'audit complets
- Anonymisation pour analyses statistiques
- Hébergement : cloud privé ou on-premise possible

**RGPD :**
- Droit à l'oubli : effacement sur demande
- Consentement explicite pour capture de données
- Transparence totale sur usage des données

---

## Organisationnel

### Mon équipe est résistante au changement. Comment convaincre ?

**Stratégie :**
1. **Commencer petit** : 1 équipe volontaire, pas toute l'organisation
2. **Montrer, ne pas dire** : Résultats concrets > promesses
3. **Impliquer tôt** : Co-construire avec l'équipe, pas imposer
4. **Célébrer les victoires** : Chaque amélioration est communiquée
5. **Transparence** : Partager aussi les échecs, apprendre ensemble

**Argument clé :** L'IA aide, ne remplace pas. Les humains restent aux commandes.

### Combien de temps avant de voir des résultats ?

**Premiers signaux (1 mois) :**
- Memory Agent réduit temps de recherche d'info
- Moins de "on avait déjà essayé ça"

**Résultats tangibles (3 mois) :**
- Patterns détectés et traités
- Décisions de meilleure qualité (simulation)
- Métriques commencent à bouger

**Transformation profonde (6-12 mois) :**
- Nouvelle culture installée
- Gains business mesurables (20-30%+)
- Le système fonctionne en autonomie

### Quels types d'organisations peuvent utiliser SYNAPSE ?

**Idéal pour :**
- Équipes tech / produit (5-50 personnes)
- Startups / scale-ups en croissance
- Départements innovation de grandes entreprises
- Cabinets de conseil (pour eux-mêmes ou clients)

**Moins adapté pour :**
- Organisations très réglementées sans marge de manœuvre
- Équipes sans compétences techniques minimum
- Contextes où l'expérimentation est impossible

**Secteurs :**
- Tech : évidemment
- Finance : possible mais réglementations complexes
- Santé : attention aux contraintes HIPAA/HDS
- Industrie : manufacturing digital, R&D

### Que se passe-t-il si un agent IA se trompe ?

**Garde-fous en place :**

1. **Les humains décident toujours** : Les agents proposent, n'imposent jamais
2. **Ethical Guardian** : Audite les décisions IA en continu
3. **Alertes** : Incohérences détectées automatiquement
4. **Traçabilité** : Toutes les décisions IA sont logged et explicables
5. **Kill switch** : Possibilité de désactiver un agent instantanément

**Si erreur :**
- Détection rapide (monitoring)
- Rollback possible
- Analyse post-mortem
- Amélioration du système

L'objectif n'est pas zéro erreur (impossible), mais résilience et apprentissage.

---

## Éthique

### L'IA ne va-t-elle pas remplacer les humains ?

**Non. Voici pourquoi :**

**Ce que l'IA fait mieux :**
- Mémoire parfaite
- Analyse de grandes quantités de données
- Détection de patterns
- Calculs et simulations

**Ce que les humains font mieux (et gardent) :**
- Définir le sens et l'intention
- Jugement éthique et contextuel
- Créativité véritable
- Relations humaines
- Décisions en incertitude radicale

SYNAPSE **augmente** les capacités humaines, ne les remplace pas.

### Comment évitez-vous les biais algorithmiques ?

**Mesures en place :**

1. **Ethical Guardian** : Rôle humain dédié à surveiller les biais
2. **Audits réguliers** : Analyse des décisions pour détecter discriminations
3. **Diversité des données** : Attention à la représentativité
4. **Transparence** : Toutes les décisions IA sont explicables
5. **Contestation** : Droit de faire appel de toute décision

**Réalisme :** Les biais existent (chez humains ET IA). L'objectif est de les détecter et corriger rapidement.

### Qu'est-ce qui empêche une organisation d'utiliser SYNAPSE pour surveiller/contrôler les employés ?

**Garde-fous éthiques :**

1. **Charte des droits** : Intégrée au framework (voir [ethics.md](../framework/ethics.md))
2. **Interdictions explicites** :
   - Pas de surveillance invasive (keylogging, etc.)
   - Pas d'évaluation individuelle par IA seule
   - Pas de scoring des personnes
3. **Transparence** : Les employés savent ce qui est capturé et pourquoi
4. **Consentement** : Adoption volontaire, pas imposée
5. **Open source** : Code auditable par tous

**Si une organisation viole ces principes :**
- Elle n'utilise plus SYNAPSE (juste les outils)
- La communauté peut la dénoncer publiquement
- Exclusion du réseau des organisations certifiées

---

## Adoption

### Par où commencer ?

1. **Lire** : [Manifeste](../MANIFESTO.md) + [Quick Start](../framework/quick-start.md)
2. **Comprendre** : [Framework complet](../framework/SYNAPSE-V0.1.md)
3. **Expérimenter** : [Guide d'implémentation](getting-started.md)
4. **Rejoindre** : [Discussions GitHub](https://github.com/synapse-origin/synapse/discussions)

**Temps estimé :** 2-3h pour comprendre, 1 semaine pour première expérimentation.

### Faut-il abandonner Scrum/Kanban pour utiliser SYNAPSE ?

**Oui, progressivement.** SYNAPSE est conçu pour remplacer les frameworks agiles existants, pas pour s'y ajouter.

**Pourquoi remplacer plutôt que compléter ?**
- Scrum a été conçu avant l'IA — ses rituels compensent l'absence de mémoire et de détection automatique
- Ajouter SYNAPSE à Scrum = double charge (rituels + agents)
- Les boucles SYNAPSE rendent les cérémonies Scrum redondantes

**Transition recommandée :**

| Phase | Durée | Ce qui change |
|-------|-------|---------------|
| **1. Hybride** | Mois 1-2 | Gardez vos sprints, ajoutez Memory Agent. Observez les redondances. |
| **2. Allègement** | Mois 3-4 | Supprimez le daily (Coordination Agent détecte). Réduisez les retros (Pattern Agent analyse). |
| **3. Remplacement** | Mois 5-6 | Les sprints deviennent optionnels. Les boucles SYNAPSE pilotent. |
| **4. SYNAPSE pur** | Mois 7+ | Plus de cérémonies Scrum. Flux continu + interventions ciblées. |

**Ce que vous gardez de l'agilité :**
- Livraison incrémentale
- Auto-organisation
- Feedback rapide
- Amélioration continue

**Ce que vous abandonnez :**
- Cycles fixes (sprints)
- Rituels calendaires (daily, retro, planning)
- Estimation manuelle (planning poker)
- Documentation manuelle des décisions

### Peut-on utiliser SYNAPSE pour un seul projet, pas toute l'organisation ?

**Oui, c'est même recommandé !**

Commencez par :
- 1 équipe / 1 projet pilote
- Périmètre limité (3-6 mois)
- Volontaires seulement
- Documentation des résultats

Si succès → extension progressive.

---

## Contribution

### Comment puis-je contribuer sans savoir coder ?

**Nombreuses façons :**

1. **Tester** : Utilisez SYNAPSE, partagez vos retours
2. **Documenter** : Améliorez la documentation, créez des guides
3. **Traduire** : Versions EN, ES, DE, etc.
4. **Évangéliser** : Parlez de SYNAPSE autour de vous
5. **Organiser** : Meetups locaux, événements communautaires
6. **Challenger** : Critiquez le framework, proposez des améliorations

Voir [CONTRIBUTING.md](../CONTRIBUTING.md) pour détails.

### Je suis chercheur. Comment mener des études sur SYNAPSE ?

**Nous encourageons la recherche académique !**

**Protocole :**
1. Contactez-nous : synapse-origin@proton.me
2. Accès aux organisations pilotes (avec leur accord)
3. Données anonymisées disponibles
4. Co-publication possible

**Thèmes de recherche :**
- Efficacité vs méthodologies agiles
- Impact sur bien-être des équipes
- Biais et éthique des systèmes hybrides
- Apprentissage organisationnel

Voir [research/](../research/) pour programme de recherche.

### Puis-je créer une entreprise autour de SYNAPSE ?

**Oui !** SYNAPSE est sous licence MIT :

**Ce que vous pouvez faire :**
- Proposer des services (conseil, formation, implémentation)
- Créer des outils commerciaux complémentaires
- Vendre du support / hosting

**Ce que vous devez faire :**
- Créditer SYNAPSE
- Contribuer les améliorations au framework (open source)
- Respecter la licence (pas de version propriétaire fermée)

**Modèles économiques possibles :**
- Conseil en transformation
- Formation et certification
- SaaS (agents hébergés)
- Support entreprise (24/7, SLA)

---

## Comparaison

### SYNAPSE vs SAFe (Scaled Agile Framework) ?

| Aspect | SAFe | SYNAPSE |
|--------|------|---------|
| **Philosophie** | Processs-driven | Intelligence-driven |
| **Coordination** | Hiérarchie + rituels | Agents IA + humains |
| **Adaptation** | Cycles trimestriels (PI) | Continue |
| **Complexité** | Très élevée (configurations multiples) | Modulaire et évolutive |
| **IA** | Absente (framework pré-IA) | Au cœur du système |

**Quand utiliser SAFe** : Grande entreprise traditionnelle, besoin de standardisation extrême  
**Quand utiliser SYNAPSE** : Organisation tech, accepte l'expérimentation, veut intégrer l'IA

### SYNAPSE vs Holacracy ?

| Aspect | Holacracy | SYNAPSE |
|--------|-----------|---------|
| **Philosophie** | Auto-gouvernance pure | Hybridation humain-IA |
| **Rôles** | Fluides, nombreux | 4 rôles fixes + agents IA |
| **Décisions** | Processus de gouvernance lourd | Simulation + décision rapide |
| **IA** | Absente | Centrale |

**Similarité** : Décentralisation du pouvoir  
**Différence** : SYNAPSE utilise l'IA pour gérer la complexité que Holacracy gère avec des processus humains lourds

### SYNAPSE vs Agile classique (Scrum) ?

Voir tableau plus haut. En résumé :
- Scrum = cycles humains fixes
- SYNAPSE = adaptation continue hybride (humains + IA)

---

## Support

### J'ai un problème technique, où demander de l'aide ?

1. **Documentation** : Cherchez dans [docs/](../docs/)
2. **FAQ** : Vous y êtes déjà !
3. **Discussions GitHub** : [Posez votre question](https://github.com/synapse-origin/synapse/discussions)
4. **Issues** : Si bug confirmé, ouvrez une [Issue](https://github.com/synapse-origin/synapse/issues)

### Je veux devenir organisation pilote, comment faire ?

**Critères :**
- Équipe tech/produit (5-50 personnes)
- Volontaires pour expérimenter (3-6 mois)
- Capacité à documenter et partager les résultats
- Compétences techniques minimum

**Processus :**
1. Contactez : synapse-origin@proton.me
2. Appel de qualification (30 min)
3. Si match : accompagnement personnalisé
4. Démarrage sous 2-4 semaines

**En échange :**
- Accès prioritaire aux nouvelles features
- Support direct des mainteneurs
- Co-construction du framework

---

**Votre question n'est pas ici ?**

👉 [Ouvrez une discussion GitHub](https://github.com/synapse-origin/synapse/discussions)
