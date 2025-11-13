# Article : Validation des données synthétiques MDClone en neuro-oncologie

## Résumé

Cet article présente une analyse comparative des résultats de données synthétiques (SD) avec les résultats d'études sur le glioblastome (GBM) et les métastases cérébrales pour évaluer la validité des données synthétiques dans la reproduction précise des tendances cliniques rapportées dans les études de cohorte originales.

---

## Méthodologie

### Tests statistiques utilisés
- **t-test** : Pour déterminer la signification statistique des écarts ou des plages
- **Analyse de survie Kaplan-Meier** : Pour évaluer les résultats de survie
- **Test du log-rank** : Pour déterminer la signification statistique
- **Ratios de risque (HR)** et **ratios de cotes** : Pour comparer les différences de survie entre sous-groupes de population
- **Test de Kolmogorov-Smirnov** : Pour évaluer la distribution des variables
- **Signification statistique** : Définie comme une valeur P inférieure à 0.05

---

## Résultats principaux

### Facteurs pronostiques pour la survie dans le glioblastome

Le GBM est une tumeur du système nerveux central de grade 4 selon l'OMS, parmi les tumeurs malignes les plus agressives chez l'adulte, caractérisée par une survie globale extrêmement faible.

#### Étude 1 : Borget et al. (2011) - Albumine sérique
- **Cohorte** : 549 patients GBM
- **Stratification** : 3 catégories basées sur les niveaux préopératoires d'albumine sérique (sAlb)
  - Hypoalbuminémie (sAlb <30 g/L)
  - Plage normale inférieure (sAlb 30-40 g/L)
  - Plage normale supérieure (sAlb >40 g/L)

**Résultats** :
- Réduction significative des taux de survie postopératoire chez les patients hypoalbuminémiques comparés aux patients avec sAlb normal (sAlb ≥30 g/L) (P<0.001)
- Patients avec sAlb normale inférieure avaient des temps de survie significativement plus courts que ceux avec sAlb dans la plage normale supérieure (P<0.001)

**Conclusion** : Le sAlb préopératoire est un puissant prédicteur de survie chez les patients GBM.

#### Étude 2 : Brown et al. (2022) - Âge et facteurs moléculaires
- **Cohorte** : 490 patients GBM
- **Stratification** : 4 groupes d'âge (<50 ans, 50-59 ans, 60-69 ans, ≥70 ans)

**Résultats** :
- Âge plus jeune significativement associé à une survie améliorée
- Chaque groupe d'âge avançant montrant des temps de survie médians progressivement plus courts
- Présence de méthylation du promoteur MGMT identifiée comme prédicteur moléculaire clé de survie plus longue

---

## Comparaison avec les données synthétiques MDClone

### Cohorte synthétique
- **452 patients** identifiés qui répondaient aux critères d'inclusion des 2 études

### Comparaison avec Borget et al. (2011)
- Distribution normale similaire avec allocation similaire à travers les 3 catégories sAlb (P=0.26)
- **Différences significatives** notées dans les caractéristiques démographiques :
  - Population synthétique démontrant un sAlb moyen plus élevé (P=0.01)
  - Âge plus élevé à la chirurgie (P<0.001)

**Modèles de traitement** :
- Dataset synthétique : proportion plus élevée de patients subissant une débulking comme approche chirurgicale primaire (63.9% vs. 47.3%)
- Étude originale : proportion plus grande de biopsies (48.6% vs. 36.1%) (P<0.001)
- **Thérapie adjuvante** : Différences significatives (P<0.001)
  - Dataset synthétique : 33.4% recevant chimiothérapie combinée
  - Étude originale : aucune thérapie multimodale

### Comparaison avec Brown et al. (2022)
- **Âge moyen** : significativement plus élevé dans le dataset synthétique (64.4±11.3 vs. 59.2±13.1 ans, P<0.001)
- **Distribution par sexe** : comparable (64.2% vs. 59.8% hommes, P=0.17)
- **Distribution par âge** : différences statistiquement significatives (P<0.01)
  - Dataset synthétique : proportion plus faible de patients <50 ans (10% vs. 22%)
  - Proportion plus élevée ≥70 ans (34% vs. 23%)

**Approches chirurgicales** : Remarquablement cohérentes entre les datasets (P=1.0)
- Biopsie : 36.1% vs. 36.0%
- Débulking : 63.9% vs. 64.0%

**Thérapie adjuvante** : Disparités significatives (P<0.001)
- Dataset synthétique : prévalence substantiellement plus élevée de chimiothérapie combinée (33.4% vs. 19.1%)

---

## Analyse de survie

### Albumine sérique
- **Corrélation substantielle** entre sAlb et survie postopératoire (P<0.001)
- Patients hypoalbuminémiques : survie postopératoire significativement plus courte
  - Médiane : 7.0 mois (95% CI: 4.8-9.3)
  - HR: 2.27 [95% CI: 1.55-3.31], P<0.01
  - Mortalité périopératoire augmentée (61.1% vs. 26.1%; OR: 4.18 [95% CI: 2.20-7.99], P<0.01)

### Âge
- Patients <50 ans : survie médiane la plus longue (16.3 mois [95% CI: 12.8-19.8])
- Patients plus âgés : temps de survie médians progressivement plus courts (P<0.001)

### Étendue de la résection
- Biopsie seule : survie médiane de 10.9 mois (95% CI: 9.6-12.3)
- Débulking : survie médiane notablement plus longue de 16.8 mois (95% CI: 14.9-18.7) (P<0.001)

---

## Métastases cérébrales

### Étude : Starzer et al. (2021)
- **Cohorte** : 1250 patients traités à l'Université médicale de Vienne entre 1990 et 2019
- **Marqueurs inflammatoires systémiques** : NLR, PLR, MLR, LLR, et ratio protéine C-réactive/albumine

### Dataset synthétique
- **1320 patients**, âge médian de 67 ans (plage: 26-95)
- **Radiothérapie** : traitement de première ligne le plus courant (77.8% vs. 51.2%, P=0.06)
- **Utilisation de stéroïdes** : proportion significativement plus élevée (55.9% vs. 38.3%, P<0.001)
- **Chimiothérapie adjuvante** : proportion significativement plus élevée (69.2% vs. 27.7%, P<0.001)

### Résultats de survie
- **NLR plus faible** (seuil: 5.07) : survie globale médiane significativement plus longue (P<0.0001)
  - 5.3 mois (95% CI: 4.5-6.2) vs. 3.7 mois (95% CI: 3.1-4.3)
- **LLR plus faible** (seuil: 5.76) : 5.0 mois vs. 3.8 mois (P<0.001)
- **PLR plus faible** (seuil: 335) : 4.5 mois vs. 3.6 mois (P=0.002)
- **MLR plus faible** (seuil: 0.53) : 4.7 mois vs. 3.7 mois (P<0.01)
- **CRP/Alb plus faible** (seuil: 2.93) : 6.7 mois vs. 3.6 mois (P<0.01)

---

## Discussion

### Applications actuelles des données synthétiques en neurochirurgie
- Analyse de tomodensitométrie
- Applications chirurgicales : planification chirurgicale améliorée, neuronavigation raffinée, visualisation chirurgicale
- Génération de preuves du monde réel pour analyses rétrospectives et études épidémiologiques

### Défis dans l'évaluation comparative et la validation
- La fiabilité des SD reste étroitement liée à la qualité et à la pertinence des données du monde réel (RWD) sous-jacentes utilisées pour les générer
- Nécessité de curation et de raffinement continus des RWD sous-jacentes

### Limitations de la taille de la cohorte et représentation des maladies rares
- Nombreux outils, tels que MDClone, imposent une exigence de taille de cohorte minimale pour garantir des corrélations statistiquement significatives
- Pour les conditions relativement rares, une seule institution peut manquer de données suffisantes

### Défis dans l'intégration des données non structurées
- Certaines variables clés étaient indisponibles, limitant notre capacité à mener toutes les analyses statistiques univariées et multivariées
- Éléments cliniques spécifiques non disponibles dans SD :
  - Génotypes tumoraux (statut de mutation IDH-1/2 ou méthylation du promoteur MGMT)
  - Étendue de la maladie métastatique extracrânienne

---

## Conclusion

Les données synthétiques ont un potentiel immense pour stimuler la recherche clinique, servant à la fois de ressource précieuse pour augmenter les données du monde réel et d'outil fiable pour générer des insights nécessaires à l'identification des tendances cliniques tout en maintenant la confidentialité des patients.

Nos résultats démontrent que les SD peuvent reproduire les corrélations du monde réel entre une variable clinique mesurable et la survie dans la recherche sur le GBM et les métastases cérébrales.

Les plateformes de synthèse de données sont essentielles pour faire progresser la recherche médicale en permettant des insights plus rapides et en facilitant un partage de données plus efficace parmi les chercheurs.

