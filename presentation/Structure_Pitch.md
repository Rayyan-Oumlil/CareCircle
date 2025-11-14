# Structure du Pitch Final - CareCircle

## ⏱️ Durée & Format

- **3 minutes** de présentation + **2 minutes** de questions (jury)
- **1-2 orateur·rices**
- **5-6 diapositives max** (hors annexes)
- **Plan B démo** : Préparer des captures statiques si besoin

## ⚠️ Clarifications Importantes (Feedback Mentor)

### Ce qui N'EST PAS attendu
- ❌ **Pas besoin d'un prototype complet** en 48h
- ❌ **Pas besoin d'un MVP fonctionnel** nécessairement
- ❌ **Pas besoin d'une démo technique** complète

### Ce qui EST attendu
- ✅ **Démontrer l'idée** : Expliquer clairement le concept
- ✅ **Montrer comment on la ferait** : Architecture, approche technique
- ✅ **Défendre l'idée** : Preuves concrètes de la nécessité
- ✅ **Valider avec utilisateurs potentiels** : Feedback de professionnels en santé mentale
- ✅ **Preuves concrètes** : Données, statistiques, témoignages

### Stratégie de Validation
- **Idée de Mouni** : Demander à des collègues en santé mentale leur avis
- **Impact** : Montrer qu'on a validé avec des professionnels du domaine
- **Argument fort** : "Nous avons consulté X professionnels qui confirment le besoin"

---

## 📊 Structure Suggerée (5-6 slides)

### Slide 1 : Problème & Impact
**Pour qui, quoi, pourquoi maintenant ?**

**Contenu suggéré :**
- **Problème** : Inégalités d'accès aux ressources en santé mentale pour intervenants de première ligne
- **Exemple concret émotionnel** : 
  > "Marie, infirmière scolaire à Rouyn-Noranda, remarque qu'un élève de 14 ans semble déprimé. Elle veut l'aider mais ne sait pas comment évaluer la situation. Les ressources spécialisées sont à 200km. Elle se sent dépassée."
- **Impact** : 
  - 50,000+ intervenants de première ligne au Québec
  - Détection tardive = problèmes plus difficiles à traiter
  - Inégalités régionales (urbain vs rural)

**Durée** : 30-40 secondes

---

### Slide 2 : Données & Approche
**Sources, variables clés, pipeline simple**

**Contenu suggéré :**
- **Données utilisées** :
  - CANPATH : Statistiques régionales, santé mentale, environnement
  - MDClone : Patterns de visites aux urgences, vagues de chaleur
  - POYM : Facteurs de risque, comorbidités psychiatriques
- **Variables clés** :
  - CANPATH : Sommeil (`SLE_*`), alcool (`ALC_*`), défavorisation (`MSD_*`), pollution
  - MDClone : Visites aux urgences, diagnostics, trajectoires de soins
  - POYM : Diagnostics psychiatriques, comorbidités
- **Pipeline simple** :
  ```
  Observations → Agents Spécialisés → Collaboration → Consensus → Réponse
  ```

**Durée** : 30-40 secondes

---

### Slide 3 : Solution & Approche Technique
**1-2 figures lisibles + comment on la ferait**

**Contenu suggéré :**
- **Concept** : Système d'agents IA multi-experts
  - 6 agents spécialisés (Red Flag, Coaching, Clinical Interview, De-escalation, Stats, Global Impact)
  - Collaboration inter-agents pour réponse fact-checked et consensus
- **Figure 1** : Diagramme de collaboration entre agents (architecture)
- **Figure 2** : Exemple visuel de réponse consolidée (mockup/diagramme)
- **Stack technique** : CrewAI, Groq API, Chroma, React
- **Interprétation** : "Un collègue expert virtuel disponible 24/7 qui combine l'expertise de 6 spécialistes en temps réel"
- **Note** : Pas besoin de démo fonctionnelle, juste montrer l'architecture et le concept

**Durée** : 45-60 secondes

---

### Slide 4 : Limites & Éthique/EDI
**Biais, qualité des données, ce que ça ne dit pas**

**Contenu suggéré :**
- **Limites** :
  - Données synthétiques (pas de données réelles confidentielles)
  - Prototype pour hackathon (validation avec experts nécessaire)
  - Pas de remplacement des professionnels, outil d'aide à la décision
  - Études existantes (ex: MH-TIPS) ont des limites de généralisation
  - Recherche future nécessaire pour évaluer faisabilité et acceptabilité
- **Éthique** :
  - Pas de stockage de données personnelles
  - Transparence sur le fonctionnement des agents
  - Respect de la confidentialité
- **Biais potentiels** :
  - Données CANPATH peuvent avoir des biais régionaux
  - Modèles LLM peuvent avoir des biais culturels/linguistiques
  - Nécessite validation avec experts diversifiés
- **Positionnement** :
  - Solution complémentaire (pas remplacement de formation continue)
  - CareCircle n'existe pas encore, offre alternative innovante

**Durée** : 30-40 secondes

---

### Slide 5 : Validation & Impact
**Preuves concrètes + qui s'en sert demain**

**Contenu suggéré :**
- **Validation avec utilisateurs potentiels** :
  - ✅ Consultation avec X professionnels en santé mentale
  - ✅ Feedback confirmant le besoin et la pertinence
  - ✅ "Nous avons validé avec des intervenants de première ligne qui confirment la nécessité"
- **Impact** :
  - Intervenants de première ligne : 50,000+ au Québec
  - Réduction des inégalités d'accès aux soins
  - Détection précoce = meilleurs résultats
- **Preuves concrètes** :
  - Données CANPATH/MDClone montrant les inégalités
  - Statistiques sur le manque de ressources en région
  - Témoignages de professionnels consultés
- **Prochaines étapes** :
  1. **Développement du prototype** : Après validation du concept
  2. **Tests pilotes** : Avec intervenants volontaires
  3. **Déploiement progressif** : Régions prioritaires

**Durée** : 40-50 secondes

---

### Slide 6 (Optionnel) : Call to Action
**Vision et impact final**

**Contenu suggéré :**
- **Vision** : "Un intervenant bien outillé dans chaque région du Québec"
- **Impact** : "Réduire les inégalités d'accès aux soins de santé mentale"
- **Innovation** : Système multi-agents collaboratifs unique pour première ligne

**Durée** : 20-30 secondes

---

## 🎯 Points Clés à Retenir

### Pour le Jury
1. **Impact et pertinence** : Problème réel, 50,000+ personnes visées, **validé avec professionnels**
2. **Originalité** : Système multi-agents collaboratifs (pas juste un chatbot)
3. **Faisabilité** : Stack technique confirmé, architecture claire
4. **Validation** : **Preuve concrète** qu'on a consulté des utilisateurs potentiels

### Pour la Présentation
- **Parler avec passion** : Le problème est réel et émotionnel
- **Montrer la validation** : "Nous avons consulté X professionnels qui confirment..."
- **Montrer l'architecture** : Diagramme de collaboration entre agents (pas besoin de démo)
- **Preuves concrètes** : Données, statistiques, témoignages de professionnels
- **Être transparent** : Mentionner les limites et l'éthique
- **Défendre l'idée** : Pourquoi c'est nécessaire, pas juste comment ça marche

---

## 📝 Checklist Avant le Pitch

- [ ] Slides créées (5-6 max)
- [ ] Timing testé (3 minutes exactement)
- [ ] Exemples concrets préparés
- [ ] Figures/diagrammes clairs et lisibles
- [ ] Plan B : Captures d'écran statiques si démo échoue
- [ ] Questions anticipées préparées
- [ ] Répétition avec l'équipe

---

## 💡 Conseils

1. **Démarrer fort** : Exemple émotionnel pour captiver l'audience
2. **Visualiser** : Diagrammes de collaboration entre agents
3. **Être honnête** : Mentionner les limites et l'éthique
4. **Avoir une vision claire** : Prochaines étapes réalistes
5. **Pratiquer** : Répéter plusieurs fois pour être à l'aise

---

## 📚 Références

- **Template fourni par Tess** : `Hackathon_RSN_Pitch_Template (1).pdf` (dans ce dossier)
- **Documentation complète** : `documentation/09_Idees_Projet_Agent_IA.md`
- **Design dashboard** : `documentation/13_Dashboard_Design_UI.md`

