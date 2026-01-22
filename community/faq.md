# ❓ Questions Fréquentes (FAQ)

---

## Général

### Qu'est-ce que SYNAPSE exactement ?

SYNAPSE est un **framework organisationnel** qui définit comment structurer la collaboration entre humains et IA. Ce n'est pas un outil ou un logiciel, mais une façon de faire fonctionner une organisation.

Il comprend :
- **4 rôles humains** (Intent Architect, Ethical Guardian, System Orchestrator, Sovereign Maker)
- **4 agents cognitifs** (Memory, Pattern, Simulation, Coordination)
- **3 boucles de feedback** (Intent Sync, Pattern Review, Decision Moment)
- **11 métriques** pour mesurer la santé du système

### En quoi c'est différent de l'agilité (Scrum, Kanban, SAFe) ?

| Aspect | Agilité Classique | SYNAPSE |
|--------|------------------|---------|
| Décisions | Humains seuls | Humains + IA |
| Adaptation | Cycles fixes (sprints) | Continue (événementielle) |
| Mémoire | Documentation manuelle | Mémoire organisationnelle persistante |
| Coordination | Rituels humains (daily, retro) | Détection automatique + intervention ciblée |
| Patterns | Détectés en rétro (trop tard) | Détection continue |

SYNAPSE ne complète pas l'agilité, il la remplace pour l'ère de l'IA.

### Peut-on utiliser SYNAPSE sans IA ?

**Partiellement, oui.** Vous pouvez adopter immédiatement :
- Les 4 rôles humains
- Les 3 boucles (comme nouveaux rituels)
- Les 11 métriques (mesurées manuellement)
- La charte éthique

Les agents IA augmentent l'efficacité mais ne sont pas obligatoires pour commencer.

### Quel est l'état actuel du projet ?

**SYNAPSE V1.0** est un framework documenté et prêt à être adopté :
- ✅ Documentation complète
- ✅ Spécifications des 4 agents
- ✅ Templates prêts à l'emploi
- ✅ Guide de transition depuis Scrum

Nous recherchons des **organisations pilotes** pour valider le framework en conditions réelles.

---

## Implémentation

### Comment implémenter les agents ?

Les agents SYNAPSE sont définis par leurs **spécifications fonctionnelles** (missions, garde-fous, interactions). L'implémentation technique est libre.

**Options possibles :**
- Outils no-code (n8n, Make, Zapier)
- LLMs via API (Claude, GPT, Mistral)
- LLMs locaux (Ollama)
- Développement custom
- Solutions sur étagère

👉 [Spécifications des agents](../framework/agents.md)

### Existe-t-il une implémentation officielle ?

**À venir.** Une solution d'implémentation SYNAPSE (cloud et on-premise) sera proposée pour les organisations souhaitant une mise en œuvre clé en main. En attendant, le framework est conçu pour être implémenté avec les outils de votre choix.

### Combien ça coûte ?

**Le framework est gratuit** (licence CC BY-SA 4.0).

Les coûts d'implémentation dépendent de vos choix :
- **Option manuelle** : 0€ (rôles + boucles sans agents)
- **Option no-code** : Variable selon les outils
- **Option LLM cloud** : Selon consommation API
- **Option locale** : Coût hardware initial, puis ~0€

### Peut-on déployer entièrement en local ?

**Oui.** Le framework est agnostique. Vous pouvez implémenter les agents avec des LLMs locaux (Ollama, etc.) pour une souveraineté totale des données.

---

## Organisationnel

### Mon équipe est résistante au changement. Comment convaincre ?

**Stratégie recommandée :**
1. **Commencer petit** : 1 équipe volontaire, pas toute l'organisation
2. **Commencer simple** : Les rôles et boucles d'abord, les agents ensuite
3. **Montrer, ne pas dire** : Résultats concrets > promesses
4. **Impliquer tôt** : Co-construire, pas imposer

**Argument clé :** L'IA aide, ne remplace pas. Les humains restent aux commandes.

### Combien de temps avant de voir des résultats ?

**1 mois :** Clarté d'intention améliorée, moins de réunions inutiles

**3 mois :** Patterns détectés et traités, décisions mieux informées

**6 mois :** Transformation visible, métriques dans le vert

### Quels types d'organisations peuvent utiliser SYNAPSE ?

**Idéal pour :**
- Équipes tech / produit (5-50 personnes)
- Startups / scale-ups
- Départements innovation
- Cabinets de conseil

**Moins adapté pour :**
- Organisations très réglementées sans marge de manœuvre
- Contextes où l'expérimentation est impossible
- Équipes sans appétence pour l'IA

### Faut-il abandonner Scrum pour utiliser SYNAPSE ?

**Transition progressive possible :**

| Phase | Durée | Ce qui change |
|-------|-------|---------------|
| Hybride | Mois 1-2 | Gardez Scrum + ajoutez les rôles SYNAPSE |
| Transition | Mois 3-4 | Réduisez les rituels, ajoutez les boucles |
| SYNAPSE | Mois 5+ | Adaptation continue, plus de cycles fixes |

👉 [Guide de transition](../docs/transition-guide.md)

---

## Éthique

### L'IA ne va-t-elle pas remplacer les humains ?

**Non.** SYNAPSE **augmente** les capacités humaines, il ne les remplace pas.

| L'IA fait mieux | Les humains gardent |
|-----------------|---------------------|
| Mémoire parfaite | Définir le sens et l'intention |
| Détection de patterns | Jugement éthique et contextuel |
| Calculs et simulations | Créativité |
| Surveillance continue | Décisions en incertitude radicale |

**Principe fondamental :** L'agent propose, l'humain décide. Toujours.

### Comment éviter les biais algorithmiques ?

**Garde-fous intégrés au framework :**
1. **Ethical Guardian** : Rôle humain dédié à l'audit
2. **Garde-fous par agent** : Ce que chaque agent ne doit PAS faire
3. **Droit de contestation** : Tout le monde peut challenger une décision IA
4. **Transparence** : Chaque proposition IA est explicable

👉 [Charte éthique complète](../framework/ethics.md)

### Qu'est-ce qui empêche la surveillance des employés ?

**Interdictions explicites dans le framework :**
- ❌ Tracking individuel minute par minute
- ❌ Comparaison des performances individuelles
- ❌ Scoring des personnes
- ❌ Surveillance hors heures de travail

**Garde-fous :**
- Ethical Guardian avec pouvoir de veto
- Charte des droits des employés
- Transparence : chacun sait ce qui est capturé

---

## Comparaisons

### SYNAPSE vs SAFe ?

| Aspect | SAFe | SYNAPSE |
|--------|------|---------|
| Philosophie | Process-driven | Intelligence-driven |
| Coordination | Hiérarchie + rituels | Agents IA + humains |
| Adaptation | Cycles trimestriels (PI) | Continue |
| IA | Absente | Au cœur du système |
| Complexité | Très élevée | Modulaire |

### SYNAPSE vs Holacracy ?

| Aspect | Holacracy | SYNAPSE |
|--------|-----------|---------|
| Philosophie | Auto-gouvernance pure | Hybridation humain-IA |
| Rôles | Fluides, nombreux | 4 rôles fixes + agents |
| Gouvernance | Processus humains lourds | IA gère la complexité |
| IA | Absente | Centrale |

---

## Adoption

### Par où commencer ?

1. **Lire** (30 min) : [SYNAPSE V1](../framework/SYNAPSE-V1.md)
2. **Identifier** les 4 rôles dans votre équipe : [Guide des rôles](../framework/roles.md)
3. **Rédiger** votre Intent Statement : [Template](../templates/intent-statement.md)
4. **Expérimenter** les 3 boucles : [Guide des boucles](../framework/loops.md)

### Comment devenir organisation pilote ?

**Critères :**
- Équipe de 5-50 personnes
- Volontaires pour expérimenter (3-6 mois)
- Capacité à documenter et partager les résultats

**En échange :**
- Accompagnement personnalisé
- Influence sur l'évolution du framework
- Visibilité (si souhaitée)

📧 Contact : synapse-origin@proton.me

### Comment contribuer ?

- **Documentation** : Améliorations, traductions
- **Templates** : Nouveaux templates utiles
- **Études de cas** : Partagez votre expérience
- **Discussions** : Questions, idées, débats

👉 [Guide de contribution](../CONTRIBUTING.md)

---

## Support

### J'ai une question, où demander ?

1. **Cette FAQ** : Vous y êtes !
2. **Documentation** : [/docs](../docs/) et [/framework](../framework/)
3. **Discussions GitHub** : [Lien](https://github.com/synapse-origin/synapse-fr/discussions)
4. **Email** : synapse-origin@proton.me

---

**Votre question n'est pas ici ?**

👉 [Ouvrez une discussion GitHub](https://github.com/synapse-origin/synapse-fr/discussions)

---

*FAQ SYNAPSE V1*  
*Dernière mise à jour : Janvier 2026*
