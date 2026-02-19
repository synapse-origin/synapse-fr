# 🤝 Guide de Contribution

Merci de contribuer à SYNAPSE !

---

## 📦 Modèle Open Core

SYNAPSE utilise un modèle Open Core :

| Composant | Licence | Contributions |
|-----------|---------|---------------|
| Documentation | CC BY-SA 4.0 | ✅ Ouvertes |
| Templates | CC BY-SA 4.0 | ✅ Ouvertes |
| Framework | CC BY-SA 4.0 | ✅ Ouvertes |
| Agents IA | Propriétaire | ❌ Fermées |

**Ce guide concerne les contributions au framework et à la documentation.**

---

## 🌟 Comment Contribuer

### 1. 📝 Documentation

Améliorez la documentation existante :
- Corrections (typos, erreurs)
- Clarifications (passages confus)
- Exemples supplémentaires
- Traductions (EN, ES, DE prioritaires)

**Fichiers concernés :** `/docs/`, `/framework/`, `/community/`

### 2. 📋 Templates

Créez ou améliorez les templates :
- Nouveaux templates utiles
- Améliorations des existants
- Adaptations sectorielles

**Fichiers concernés :** `/templates/`

### 3. 📊 Études de Cas

Partagez votre expérience :
- Retours d'implémentation
- Métriques avant/après
- Leçons apprises

**Fichiers concernés :** `/case-studies/`

### 4. 💡 Idées & Discussions

Proposez des améliorations au framework :
- Nouveaux concepts
- Ajustements méthodologiques
- Questions et débats

👉 **[GitHub Discussions](https://github.com/synapse-origin/synapse/discussions)**

### 5. 🔬 Recherche

Contribuez au programme de recherche :
- Propositions d'études
- Analyses académiques
- Publications

**Fichiers concernés :** `/research/`

---

## 🔄 Workflow

### Pour Documentation & Templates

```bash
# 1. Fork le repository
# (via GitHub)

# 2. Clone votre fork
git clone https://github.com/VOTRE-USERNAME/synapse.git
cd synapse

# 3. Créez une branche
git checkout -b docs/ma-contribution

# 4. Faites vos modifications
# (éditez les fichiers)

# 5. Commit
git add .
git commit -m "docs: améliore section X"

# 6. Push
git push origin docs/ma-contribution

# 7. Ouvrez une Pull Request
# (via GitHub)
```

### Conventions de Commit

```
docs: pour documentation
template: pour templates
case-study: pour études de cas
research: pour recherche
fix: pour corrections
```

**Exemples :**
- `docs: clarifie la section Intent Sync`
- `template: ajoute template onboarding`
- `fix: corrige typo dans metrics.md`

---

## 📋 Standards

### Documentation

- **Langue principale :** Français
- **Format :** Markdown
- **Style :** Clair, concret, avec exemples
- **Structure :** Headers hiérarchiques, liens internes

### Templates

- **Format :** Markdown
- **Instructions :** Incluses en commentaires
- **Exemples :** Au moins un exemple rempli
- **Compatibilité :** Utilisable sans les agents IA

### Études de Cas

- **Template :** Utiliser `/case-studies/template.md`
- **Métriques :** Quantifiées si possible
- **Anonymisation :** Possible si souhaitée
- **Honnêteté :** Inclure aussi les échecs

---

## ✅ Checklist Pull Request

Avant de soumettre :

- [ ] J'ai lu ce guide de contribution
- [ ] Ma contribution concerne la documentation/templates (pas le code des agents)
- [ ] J'ai vérifié l'orthographe et la grammaire
- [ ] Les liens internes fonctionnent
- [ ] J'ai testé les exemples/templates
- [ ] Le commit message suit les conventions
- [ ] J'accepte que ma contribution soit sous licence CC BY-SA 4.0

---

## 🌍 Traductions

### Langues Prioritaires

1. **Anglais (EN)** - Haute priorité
2. **Espagnol (ES)** - Moyenne priorité
3. **Allemand (DE)** - Moyenne priorité

### Comment Traduire

1. Créez un dossier `/docs/[lang]/` (ex: `/docs/en/`)
2. Traduisez les fichiers principaux d'abord :
   - `README.md`
   - `framework/SYNAPSE-V0.1.md`
   - `framework/quick-start.md`
3. Gardez la même structure de fichiers
4. Adaptez les exemples au contexte culturel si pertinent

### Coordination

Avant de commencer une traduction :
1. Vérifiez dans les [Issues](https://github.com/synapse-origin/synapse/issues) si quelqu'un n'a pas déjà commencé
2. Créez une Issue pour signaler que vous commencez
3. Utilisez les [Discussions](https://github.com/synapse-origin/synapse/discussions) pour coordonner

---

## 🏢 Devenir Organisation Pilote

Une autre façon de contribuer : tester SYNAPSE en conditions réelles.

**Ce que vous apportez :**
- Retours terrain
- Validation du framework
- Études de cas

**Ce que vous recevez :**
- Accompagnement privilégié
- Accès early aux agents (quand disponibles)
- Influence sur la roadmap

📧 **Contact :** synapse-origin@proton.me

---

## ❓ Questions Fréquentes

### Puis-je contribuer du code ?

Le code des agents IA n'est pas ouvert aux contributions. Vous pouvez contribuer à la documentation, templates, et études de cas.

### Puis-je créer mes propres agents basés sur les specs ?

Oui, vous pouvez créer vos propres implémentations. Vous ne pouvez pas les appeler "SYNAPSE Agent" ni prétendre qu'ils sont officiels.

### Comment sont validées les contributions ?

Les Pull Requests sont revues par les mainteneurs. Critères :
- Qualité du contenu
- Cohérence avec le framework existant
- Respect des standards

### Puis-je être rémunéré pour contribuer ?

Pas de programme de rémunération actuellement. Les contributions significatives sont créditées et peuvent ouvrir des opportunités (partenariats, consulting).

---

## 📞 Contact

**Questions sur les contributions :**  
💬 [GitHub Discussions](https://github.com/synapse-origin/synapse/discussions)

**Devenir pilote :**  
📧 synapse-origin@proton.me

**Partenariats :**  
📧 synapse-origin@proton.me

**Général :**  
📧 synapse-origin@proton.me

---

## 🙏 Remerciements

Chaque contribution, même petite, fait avancer SYNAPSE.

Les contributeurs sont listés dans [CONTRIBUTORS.md](CONTRIBUTORS.md) *(à créer après premières contributions)*.

---

**Merci de faire partie de l'aventure SYNAPSE !**

---

*Guide de contribution - SYNAPSE*  
*Dernière mise à jour : Novembre 2025*
