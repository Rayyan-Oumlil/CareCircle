# Questions de recherche pour générer des bases de données dans MDClone

## Question 1 : Conditions socio-économiques et hospitalisations évitables

**Question** : Comment les conditions socio-économiques influencent-elles les hospitalisations évitables pour les maladies chroniques ?

### Variables clés à inclure

**Démographiques** :
- Âge, sexe, code postal, langue principale

**Socioéconomiques** :
- Revenu médian du quartier, statut d'emploi, type de logement

**Cliniques** :
- Diagnostic principal (diabète, MPOC|BPCO, insuffisance cardiaque, HTA)
- Comorbidités, durée du séjour

**Utilisation des soins** :
- Nombre de visites à l'urgence
- Réadmissions à 30 jours
- Suivi en première ligne

### Applications possibles
- Modèle de prédiction d'hospitalisation évitable
- Tableau de bord des inégalités territoriales

---

## Question 2 : Complications cardiovasculaires chez les patients diabétiques

**Question** : Quels facteurs prédisent les complications cardiovasculaires chez les patients diabétiques ?

### Variables clés à inclure

**Diagnostic principal** :
- Diabète type 2

**Variables cliniques** :
- HbA1c, cholestérol, IMC, pression artérielle

**Médications** :
- Insuline, statines, antihypertenseurs

**Issue** :
- Infarctus, AVC, hospitalisation d'urgence

**Facteurs comportementaux** :
- Tabac, activité physique (si disponible)

### Applications possibles
- Modèle prédictif de complication
- Segmentation de cohorte diabétique

---

## Question 3 : Trajectoire de soins - Insuffisance cardiaque

**Question** : Quelle est la trajectoire de soins des patients atteints d'insuffisance cardiaque dans les 12 mois suivant un premier épisode ?

### Variables clés à inclure

- Diagnostic d'insuffisance cardiaque
- Dates d'admission, réadmission, visites à l'urgence
- Médication : diurétiques, inhibiteurs ACE, bêta-bloquants
- Variables sociodémographiques : âge, sexe
- Issue : décès, hospitalisation prolongée

### Applications possibles
- Analyse de parcours patient
- Identification de points critiques dans la prise en charge

---

## Question 4 : Perte d'autonomie chez les personnes âgées

**Question** : Quels facteurs cliniques et sociaux prédisent la perte d'autonomie à la sortie d'hospitalisation chez les personnes âgées ?

### Variables clés à inclure

- Âge ≥ 65 ans, sexe, fragilité (score ou indicateur dérivé)
- Diagnostic : chutes, fractures, dépression, démence
- Durée du séjour, soins reçus (ergothérapie, réadaptation)
- Destination post-sortie : domicile, CHSLD, centre de réadaptation
- Réadmission à 30 jours

### Applications possibles
- Outil de triage clinique pour gestion du risque
- Tableau de bord de fragilité gériatrique

---

## Question 5 : Polymédication et réadmission

**Question** : Les patients âgés polymédicamentés présentent-ils un risque accru de réadmission hospitalière ?

### Variables clés à inclure

- Nombre de médicaments prescrits (>5)
- Diagnostics chroniques principales
- Âge, sexe, durée du séjour
- Réadmission 30/90 jours
- Indice de fragilité, comorbidités

### Applications possibles
- Modélisation du risque de réadmission liée à la polymédication
- Stratégie de déprescription ciblée

---

## Question 6 : Transparence des données synthétiques

**Question** : Comment assurer la transparence et la traçabilité des jeux de données synthétiques utilisés en recherche clinique ?

### Variables clés à inclure

**Métadonnées** :
- Source du jeu, méthode de génération (MDClone), date de création
- Niveau d'anonymisation, licence d'accès, fréquence de mise à jour

**Indicateurs d'usage** :
- Nombre de requêtes, utilisateurs, thématique

**Variables simulées** :
- Structure, distribution, corrélation

### Applications possibles
- Prototype de registre de transparence des données
- Cadre de gouvernance pour la recherche responsable

---

## Question 7 : Indicateurs de santé respectueux des principes OCAP

**Question** : Comment développer des indicateurs de santé respectueux des principes OCAP (Ownership, Control, Access, Possession) ?

### Variables clés à inclure

- Données agrégées par région ou communauté (synthétiques)
- Indicateurs de santé : dépistage, maladies chroniques, vaccination, hospitalisations
- Variables sociales : logement, emploi, isolement géographique, accès aux soins
- Métadonnées : consentement simulé, source, méthode d'agrégation

### Applications possibles
- Tableau de bord de gouvernance participative
- Outil de simulation des impacts d'un modèle OCAP

---

## Question 8 : Vagues de chaleur et hospitalisations

**Question** : Les vagues de chaleur estivales augmentent-elles le risque d'hospitalisation pour maladies respiratoires et cardiovasculaires ?

### Variables clés à inclure

- Dates d'admission et de sortie
- Diagnostic principal : MPOC, asthme, infarctus, insuffisance cardiaque
- Données environnementales : température quotidienne, humidex, indice AQI (qualité de l'air)
- Code postal, âge, sexe

### Applications possibles
- Analyse temporelle de l'effet chaleur/santé
- Tableau de bord climat-santé pour Montréal

---

## Question 9 : Pollution atmosphérique et MPOC

**Question** : Les journées de forte pollution atmosphérique sont-elles associées à une augmentation des admissions pour MPOC chez les personnes âgées ?

### Variables clés à inclure

- Âge ≥ 65 ans, sexe, code postal
- Diagnostic : MPOC, bronchite chronique
- Date d'admission, durée d'hospitalisation
- AQI (niveau de pollution), température moyenne (à avoir avec CANUE ?)

### Applications possibles
- Étude corrélationnelle pollution-hospitalisations
- Prototypage d'un outil de surveillance environnementale

---

## Question 10 : Défavorisation et réadmissions

**Question** : Existe-t-il un lien entre la défavorisation matérielle et la fréquence des réadmissions hospitalières à 30 jours ?

### Variables clés à inclure

- Âge, sexe, code postal (lié à un indice de défavorisation)
- Diagnostic d'admission, date d'admission et de sortie
- Nombre de réadmissions (30, 90 jours)
- Statut de résidence (urbain/rural), accès à un médecin de famille

### Applications possibles
- Visualisation géospatiale des réadmissions
- Analyse de réadmission selon le gradient social

