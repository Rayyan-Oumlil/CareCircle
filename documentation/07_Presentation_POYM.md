# POYM - Prédiction du risque de mortalité hospitalière à un an

## Informations générales

**Auteur** : Hakima Laribi  
**Statut** : Étudiante au doctorat, Département d'informatique, Université de Sherbrooke

**Superviseurs** :
- Martin Vallières, Professeur associé, Département d'Oncologie, Université McGill
- Dan Poenaru, Professeur associé, Département de Chirurgie pédiatrique, Hôpital pour enfants de Montréal

---

## Contexte

### Citation clé
> "Prédire l'espérance de vie des patients individuels peut être important à la fois pour la prise de décision médicale et pour la recherche"  
> [Carl van Walraven et al., 2015]

### Statistiques canadiennes
Parmi un échantillon d'environ 1/3 des Canadiens :
- **56%** sont morts à l'hôpital
- **26%** ont connu une admission aux soins intensifs lors de leur dernière visite
- **75%** ont été vus par >10 médecins dans les 6 derniers mois

**Source** : Fowler, R., & Hill, A. (2018). A National Comparison of Intensity of End-Of-Life Care in Canada

### Préférences des familles
Cependant, lors d'enquêtes auprès des familles de patients décédés à l'hôpital :
- **72%** préfèrent un décès hors de l'hôpital
- "Certains" patients reçoivent des soins qui ne correspondent pas à leurs préférences

**Conclusion** : Il est important d'initier des discussions sur les objectifs de soins avec les patients en fin de vie

---

## Discussions sur les objectifs de soins (GOC)

### Questions clés
- Le patient veut-il être réanimé ?
- Le patient veut-il être intubé ?
- Le patient veut-il procéder à des soins potentiellement agressifs ?
- Le patient préfère-t-il commencer les soins palliatifs ?

### Besoin identifié
1. Il est important d'initier des discussions sur les objectifs de soins avec les patients en fin de vie
2. **Nous devons identifier les patients à haut risque de mortalité tôt**

---

## Modèles de prédiction de mortalité

### HOMR (Hospital One-year Mortality Risk)
- **HOMR** : Prédiction de mortalité à un an post-décharge
- **mHOMR** : Prédiction de mortalité à un an pendant l'admission
- **RF-HOMR** : Prédiction de mortalité à un an pendant et/ou à l'admission
- **HOMR Now!** : Identification automatisée des patients à haut risque de mortalité à un an

**Utilise** : Données administratives collectées dans les dossiers de santé électroniques (EHR) des patients

### ELN (Enhanced Learning Network)
- **Auteur** : Laribi et al., 2025

---

## Dataset

### Dataset original
- **Source** : CIUSSS de l'Estrie-CHUS, Sherbrooke, Canada
- **Période** : 1er juillet 2011 – 30 juin 2021
- **Patients** : 123,646 patients
- **Hospitalisations** : 250,812 hospitalisations
- **Mortalité à un an** : ~15% des patients

### Dataset synthétique
- **Patients** : 123,646 patients
- **Hospitalisations** : 248,485 hospitalisations
- **Disponibilité** : Publiquement disponible
- **Méthode** : Mapper chaque patient à un patient synthétique en utilisant la méthode AVATAR (Guillaudeux et al., 2023)
- **Dataset privé** : En partenariat avec Octopize.io

**Groupe de patients synthétiques** avec les mêmes propriétés statistiques que les patients originaux.

**Comparaison détaillée** : https://www.researchsquare.com/article/rs-5363467/v1  
**Dataset synthétique** : https://zenodo.org/records/12954673

---

## Variables du dataset

### 244 prédicteurs incluant :

#### Démographiques
- Âge, sexe

#### Caractéristiques d'admission
- Type d'admission, service d'admission, si admis par ambulance, etc.

#### Diagnostics d'admission
- Diagnostics émis à l'admission : `adm_*`

#### Diagnostics de comorbidité
- Diagnostics émis lors d'admissions précédentes : `dischargedx_*`

---

## Challenge

### Tâche
Deux classificateurs Random Forest ont été entraînés pour prédire le risque de mortalité à un an des patients.

**Votre tâche** : Post-analyser la performance de chaque modèle pré-entraîné :
- Un entraîné sur un sous-ensemble du dataset synthétique
- Un autre entraîné sur le dataset original complet

### Évaluation
Les deux modèles seront évalués sur une fraction du dataset synthétique, et leurs résultats seront comparés pour évaluer les différences de performance, de généralisation et de biais potentiels.

**Code** : https://github.com/LaribiHakima/rsn_challenge

