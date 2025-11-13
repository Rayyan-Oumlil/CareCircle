# Présentation MDClone - MUHC

## Structure RI-MUHC 2023

### Data Warehouse (DW)
- **Patient-centred database** liée avec un épisode de soins au MUHC
- **Types d'épisodes** : Pre-admit, Inpatient, Day surgery, Emergency, Outpatient, Radio-oncology
- **Sites MUHC** : MGH, RVH, MNH, MCI, MCH, LAC
- Processus établi pour l'accès aux données de recherche
- Équipe à temps plein d'analystes avec expertise en recherche et méthodes pour créer des datasets

---

## Terminologie MUHC

### Vocabulaire médical
Les vocabulaires médicaux sont des terminologies pour enregistrer les constatations, circonstances, événements ou interventions des patients avec suffisamment de détails pour supporter les soins cliniques, l'aide à la décision, la recherche sur les résultats et la qualité.

### Standards internationaux
- **Diagnostics** : ICD-9/10 (CA) / DRG / CCI* → ICD-10/11, DRG, SNOMED
- **Procédures** : SNOMED
- **Médicaments** : AHFS**/DINs → AHFS/RxNorm
- **Concepts de laboratoire (LIS)** : LOINC
- **Images** : DICOM → DICOM

*Canadian Classification of Health Interventions  
**American Hospital Formulary Service

---

## Données synthétiques

### Qu'est-ce que c'est ?
Les données synthétiques sont des données **non réversibles**, créées artificiellement, qui répliquent les caractéristiques statistiques et les corrélations des données brutes du monde réel.

En utilisant des variables discrètes et non discrètes d'intérêt, les données synthétiques ne contiennent **pas d'informations identifiables** car elles utilisent une approche statistique pour créer un tout nouveau dataset.

Alors qu'un individu avec des données anonymisées ou désidentifiées peut être identifié en inférant des caractéristiques, en croisant des similarités de données, ou en inversant l'approche des données, les données synthétiques sont la **seule méthode d'anonymisation qui empêche entièrement la ré-identification**.

### Avantages vs Limitations

#### Avantages
- Études de recherche rétrospectives
- Explorer les données indépendamment du processus IRB
- Accès aux données instantanément
- Explorer les données dynamiquement
- Maintenir la confidentialité des patients
- Partager les données dans le monde entier
- Idéal pour les tests d'Intelligence Artificielle

#### Limitations
- Pas utile pour les études de perspectives
- Minimum de 200 patients dans la population
- Certaines informations ne sont pas disponibles avec les données synthétiques :
  - Images
  - Variables catégorielles censurées en pourcentage élevé (plus spécifique = plus censuré)
  - Événements répétitifs multiples non disponibles
  - Texte libre et autres variables pourraient être trouvés dans des langues locales

---

## MDClone - Quand l'utiliser et comment y accéder ?

### Quand utiliser les données synthétiques vs données réelles

#### MDClone (Données synthétiques)
- Idéal pour explorer la faisabilité et planifier des projets de recherche
- Recommandé comme première étape avant de demander des données au niveau patient réel

#### Data Warehouse (Données agrégées, anonymisées, désidentifiées ou identifiables)
- Utiliser lorsque des données au niveau patient réel sont nécessaires
- Nécessite l'approbation du REB et l'autorisation finale de la Personne Mandatée avant l'accès, sauf pour les données agrégées

### Accès à MDClone
- Les cliniciens et employés du MUHC peuvent demander l'accès
- Les identifiants MUHC et l'accès au réseau sont requis
- Envoyer un email à **santiago.marquez@muhc.mgill.ca** avec UNI, département et position

---

## Description des datasets

### Dataset 1 : Prédiction d'admission hospitalière
**Question** : Quelle est la précision de la prédiction d'admission hospitalière pour les patients âgés de 65 ans et plus qui visitent le service d'urgence ?

- **Événement** : Admission du patient aux urgences, 65 ans ou plus
- **Résultat** : Admission hospitalière (Oui/Non)
- **Variables** : Âge, Sexe, Comorbidités, Signes vitaux à la visite aux urgences

---

### Dataset 2 : Complications cardiovasculaires chez les patients diabétiques
**Question** : Quels facteurs prédisent les complications cardiovasculaires chez les patients diabétiques ?

- **Événement (Condition)** : Patients avec diagnostic de diabète de type 2 chez les individus âgés de 18 ans et plus
- **Variables cliniques** : Premier résultat de laboratoire de HbA1c, cholestérol, glycémie, homocystéine, triglycérides et créatinine, collecté dans les 90 jours après l'événement (condition)
- **Année de naissance, sexe à la naissance**
- **Résultats** :
  - a) AVC, insuffisance cardiaque et insuffisance rénale chronique, évalués jusqu'à 10 ans après l'événement (condition)
  - b) Visites aux urgences, évaluées jusqu'à 1 an après l'événement

---

### Dataset 3 : Vagues de chaleur estivales
**Question** : Les vagues de chaleur estivales augmentent-elles le risque d'hospitalisations pour maladies respiratoires et cardiovasculaires ?

- **Événement** : Admission à l'hôpital avec l'un des codes ICD-10 suivants comme diagnostic principal :
  - MPOC : J41–J44
  - Asthme : J45
  - Infarctus aigu du myocarde : I21–I22
  - Insuffisance cardiaque : I50
- **Temps d'événement** : admission_month
- **Variables** : genre, âge, LOS (durée de séjour)
- **Données liables** : Données environnementales : température quotidienne, humidex, indice de qualité de l'air (AQI)

---

### Dataset 4 : Pollution atmosphérique et MPOC
**Question** : Les journées de forte pollution atmosphérique sont-elles associées à une augmentation des admissions pour MPOC chez les personnes âgées ?

- **Événement** : Admission à l'hôpital pour patients adultes de 65 ans et plus, avec l'un des codes ICD-10 suivants comme diagnostic principal : MPOC : J41–J44 (adultes de 65 ans et plus)
- **Temps d'événement** : admission_month
- **Variables** : Sexe à la naissance, âge, LOS
- **Données liables** : Données environnementales : indice de qualité de l'air (AQI), température moyenne

