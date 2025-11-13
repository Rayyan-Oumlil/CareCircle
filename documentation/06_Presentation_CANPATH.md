# Présentation CANPATH - Données synthétiques

## Convention de nommage des variables

### Démographiques des participants
- Préfixe : `SDC_`

### État de santé
- Préfixe : `HS_`

### Conditions médicales et maladies
- Préfixe : `DIS_`

### Comportements
- **Sommeil** : `SLE_`
- **Alcool** : `ALC_`
- **Tabac** : `SMK_`
- **Nutrition** : `NUT_`
- **Activité physique** : `PA_`

### Statut de travail
- Préfixe : `WRK_`

### Mesures anthropométriques
- Préfixe : `PM_`

### COVID-19
- Préfixe : `C_`

---

## Données de base et maladies supplémentaires

### Questionnaire sur les maladies supplémentaires
Variables supplémentaires (`DIS_`) de trois des cinq cohortes basées sur la population de CanPath, incluant des informations sur :

- **Santé auditive**
- **Santé visuelle**
- **Santé bucco-dentaire**

### Student Dataset
Le Student Dataset comprend **200+ variables**, telles que :

- `DIS_EYE_DIAB_RET_EVER` : Occurrence de rétinopathie diabétique à tout moment pendant la vie du participant
- `DIS_EYE_DIAB_RET_AGE` : Âge du participant au diagnostic de rétinopathie diabétique

---

## Variables CANUE

### Environnement bâti et social
- **Densité des points de vente alimentaires et de détail** : `NHFED_09-32`
- **Environnement de vie active** : `ALE_06-07`
- **Indice de défavorisation matérielle et sociale** : `MSD_08-09`
- **Couverture de la canopée d'arbres** : `GRTCC_01-05`
- **Indice de végétation par différence normalisée** : `GRLAN_09`

### Température
- **Températures annuelles les plus élevées, les plus basses et moyennes** : `WTHNRC_01-03`
- **Températures quotidiennes moyennes max/min** : `WTHNRC_04-05`

### Pollution atmosphérique
- **PM2.5 moyenne annuelle** : `PM25DAL_01`
- **NO2 moyenne annuelle** : `NO2LUR_02`
- **SO2 moyenne sur 3 ans** : `SO2OMI_01`
- **O3 moyenne sur 8 heures en saison chaude** : `O3CHG_04`

### Autres
- **Luminosité de la lumière nocturne** : `LGTNLT_01`
- **Distance à la frontière de la division de recensement** : `NO2LUR_05`
- **Variables de densité des points de vente alimentaires et de détail** : `NHFED_09-32`

---

## Cas d'utilisation

### Pilote (Automne 2020) – Dr. Jennifer Brooks

**Cours** : Analyse quantitative pour les étudiants en épidémiologie MPH

**Citation** :
> "L'utilisation du dataset synthétique CanPath a fait une énorme différence ! Maintenant, 95% de nos étudiants le préfèrent pour leurs projets. Il les aide à explorer une large gamme de questions de recherche, de l'exposition environnementale à l'apport alimentaire, et de l'anxiété aux migraines. L'augmentation de l'engagement a été incroyable !"

**Dr. Jennifer Brooks**, Directrice exécutive de CanPath & Professeure adjointe U of T

**Analyses effectuées** :
- Anxiété et migraines
- Fruits et légumes alimentaires et cancer colorectal
- Horaire de travail et consommation excessive d'alcool

**Méthodes utilisées** : Ratios de cotes, analyses de corrélation, et plus

---

### Épidémiologie II - Dr. Daniel Fuller

**Cours** : Community Health & Epidemiology

**Objectif** : Introduire et appliquer l'ajustement de modèles, la modification de la mesure d'effet et l'interprétation en utilisant des données synthétiques du monde réel

**Résultat** : Renforcement des concepts de base en régression, confusion et interaction dans le contexte de la santé de la population

**Plateforme** : Analyses effectuées en R ou Stata pendant les sessions de laboratoire

**Citation** :
> "Spécifiquement, la taille du dataset, la gamme de variables et les aspects des données manquantes font du dataset idéal pour apprendre l'épidémiologie avancée et la science des données. Avoir un dataset cohérent et complet que les étudiants utilisent pendant tout un cours signifie que nous pouvons approfondir les sujets plus rapidement et passer moins de temps à apprendre de nouveaux datasets pendant le cours."

**Dr. Daniel Fuller**, Professeur associé, Université de Saskatchewan

**GitHub** : https://github.com/walkabilly/chep801_usask

---

### AI4PH Summer Institute – Student Data Challenge

**Exemples d'études** :
- Association entre dépression et maladie cardiovasculaire
- Activité physique et santé générale auto-perçue chez les adultes atteints d'arthrose
- Risque de développer le diabète de type II comparé chez les adultes blancs vs noirs

**Citation** :
> "Ce défi de données, développé en utilisant le dataset synthétique CanPath, est une opportunité de formation incroyable pour introduire efficacement des techniques d'inférence causale avancées et comment elles peuvent être appliquées à des études de santé complexes utilisant des données du monde réel"

**Dr. Kuan Liu**, Mentor AI4PH et Professeur adjoint U of T

---

## Notes importantes

- **Ne pas utiliser pour publication**
- Les étudiants intéressés à découvrir si les résultats de leur projet peuvent être répliqués en utilisant les données réelles de CanPath pour une publication potentielle peuvent demander l'accès aux données via le processus d'accès régulier de CanPath
- **Frais réduits disponibles** pour les étudiants et stagiaires demandant l'accès aux données et échantillons biologiques de CanPath

