# Pattern Report #[ID]

**Date de détection** : [JJ/MM/AAAA]  
**Détecté par** : Pattern Agent  
**Type** : ☐ Négatif (Problème) ☐ Positif (Opportunité) ☐ Neutre (Information)  
**Sévérité** : ☐ Faible ☐ Moyenne ☐ Haute ☐ Critique  
**Status** : ☐ Nouveau ☐ Analysé ☐ Action en cours ☐ Résolu ☐ Ignoré

---

## 📊 Résumé Exécutif

**En une phrase** : [Description du pattern en 1 phrase]

**Impact estimé** : [Quantitatif si possible - ex: +3 jours délai, -20% performance, etc.]

**Recommandation** : ☐ Action immédiate ☐ Planifier ☐ Monitorer ☐ Ignorer

---

## 🔍 Description du Pattern

### Nature du Pattern

[Décrire le pattern de façon détaillée : qu'est-ce qui se répète ? Dans quel contexte ? Depuis quand ?]

**Exemple** :
```
"Feature Y prend systématiquement 2x plus de temps que estimé"

ou

"Les bugs critiques résolus en pair programming sont fixés 40% plus vite"
```

---

## 📈 Données & Métriques

### Fréquence

**Occurrences détectées** : [Nombre]  
**Période observée** : [Du JJ/MM/AAAA au JJ/MM/AAAA]  
**Tendance** : ☐ Croissante ☐ Stable ☐ Décroissante

**Historique** :

| Date | Occurrence | Contexte |
|------|-----------|----------|
| [Date 1] | [Description] | [Contexte] |
| [Date 2] | [Description] | [Contexte] |
| [Date 3] | [Description] | [Contexte] |
| ... | ... | ... |

---

### Impact Quantifié

**Coût** :
- Temps perdu : [X heures/jours]
- Coût financier : [X €]
- Opportunité manquée : [Description]

**Personnes/Équipes Impactées** :
- [Équipe A] : [Impact]
- [Équipe B] : [Impact]
- [Personne X] : [Impact]

**Métriques Affectées** :

| Métrique | Avant | Avec Pattern | Écart |
|----------|-------|--------------|-------|
| [Ex: Temps de cycle] | [X jours] | [Y jours] | [+Z jours] |
| [Ex: Vélocité] | [X points] | [Y points] | [-Z%] |
| [Ex: Bugs production] | [X%] | [Y%] | [+Z%] |

---

## 🧠 Analyse des Causes

### Causes Racines Identifiées

**Méthode utilisée** : ☐ 5 Whys ☐ Fishbone ☐ Analyse stats ☐ ML clustering

**Analyse** :

1. **Cause Racine #1** : [Description]
   - Contributeurs : [Facteurs qui contribuent]
   - Preuve : [Données qui supportent]

2. **Cause Racine #2** : [Description]
   - Contributeurs : [Facteurs]
   - Preuve : [Données]

**Exemple - 5 Whys** :
```
Problème : Feature Y prend 2x plus de temps

Pourquoi 1 ? → Tests end-to-end compliqués
Pourquoi 2 ? → Beaucoup de dépendances externes
Pourquoi 3 ? → Architecture trop couplée
Pourquoi 4 ? → Pas de refactoring depuis 2 ans
Pourquoi 5 ? → Dette technique non priorisée

Cause Racine : Dette technique non gérée
```

---

### Contexte & Déclencheurs

**Conditions nécessaires** :
- [Condition 1 qui fait apparaître le pattern]
- [Condition 2]

**Déclencheurs** :
- [Événement qui déclenche]

---

## 🎯 Recommandations

### Option A : [Nom de l'option]

**Description** : [Que faire ?]

**Bénéfices attendus** :
- [Bénéfice 1]
- [Bénéfice 2]
- [Bénéfice 3]

**Coût de mise en œuvre** :
- Temps : [X jours/semaines]
- Ressources : [Personnes nécessaires]
- Budget : [€]

**Risques** :
- [Risque 1]
- [Risque 2]

**Priorité** : ☐ Haute ☐ Moyenne ☐ Basse

---

### Option B : [Nom de l'option]

[Même structure que Option A]

---

### Option C : Ignorer

**Justification** :
- [Pourquoi on pourrait ignorer]
- [Coût correction > Bénéfice]

---

## ✅ Décision Prise

**Date de décision** : [JJ/MM/AAAA]  
**Décideur** : [System Orchestrator / Intent Architect / Autre]

**Option choisie** : [Option A / B / C / Autre]

**Justification** :
[Pourquoi cette option a été choisie]

---

## 📋 Plan d'Action

### Actions Immédiates (< 7 jours)

- [ ] [Action 1] - Responsable : [Nom] - Date : [JJ/MM]
- [ ] [Action 2] - Responsable : [Nom] - Date : [JJ/MM]

### Actions Moyen Terme (< 30 jours)

- [ ] [Action 1] - Responsable : [Nom] - Date : [JJ/MM]
- [ ] [Action 2] - Responsable : [Nom] - Date : [JJ/MM]

### Mesures Préventives

- [ ] [Mesure pour éviter récurrence]
- [ ] [Mesure pour détecter plus tôt]

---

## 📊 Métriques de Suivi

**Comment mesurer le succès de l'action ?**

| Métrique | Baseline | Cible | Deadline | Responsable |
|----------|----------|-------|----------|-------------|
| [Ex: Temps feature Y] | 10 jours | < 6 jours | M+2 | [Nom] |
| [Ex: Taux bugs] | 5% | < 3% | M+3 | [Nom] |

---

## 🔄 Suivi & Résultats

### Revue #1 (Date : [JJ/MM/AAAA])

**Avancement** : [X%]

**Actions complétées** :
- [Action 1] ✅
- [Action 2] 🟡 En cours

**Métriques** :

| Métrique | Baseline | Actuel | Cible | Status |
|----------|----------|--------|-------|--------|
| [Métrique 1] | [X] | [Y] | [Z] | ☐ ✅ ☐ 🟡 ☐ ❌ |

**Observations** :
[Ce qu'on observe]

**Ajustements** :
[Si nécessaire]

---

### Revue #2 (Date : [JJ/MM/AAAA])

[Même structure que Revue #1]

---

## 🎓 Apprentissages

### Ce Qui a Fonctionné

- [Élément 1]
- [Élément 2]

### Ce Qui N'a Pas Fonctionné

- [Élément 1]
- [Élément 2]

### Pour la Prochaine Fois

**À faire** :
- [Recommandation 1]
- [Recommandation 2]

**À éviter** :
- [Anti-pattern 1]
- [Anti-pattern 2]

---

## 🔗 Liens

**Patterns similaires** :
- [Pattern Report #XX] - [Titre]
- [Pattern Report #YY] - [Titre]

**Décisions liées** :
- [Decision Record #XX] - [Titre]
- [Decision Record #YY] - [Titre]

**Ressources** :
- [Lien vers analyse détaillée]
- [Lien vers données]

---

## 📝 Notes & Commentaires

### [Date] - [Auteur]
[Note ou commentaire]

### [Date] - [Auteur]
[Note ou commentaire]

---

## 📎 ANNEXES

### Annexe A : Données Brutes

[Tableaux, graphiques, logs, etc.]

### Annexe B : Analyse Statistique

[Si analyse ML ou stats poussées]

### Annexe C : Code/Configurations

[Si changements techniques]

---

*Pattern Report maintenu par System Orchestrator et Pattern Agent*  
*Ce document doit être mis à jour au fil de l'implémentation des actions*
