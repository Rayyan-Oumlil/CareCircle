# Projet de recherche proposé

## Questions de recherche pour générer des bases de données dans MDClone

### Question 1 : Conditions socio-économiques et hospitalisations évitables

**Question** : How do socioeconomic conditions influence avoidable hospitalizations for chronic diseases?

**Key variables** :
- Demographics: age, sex, postal code, primary language
- Socioeconomic: neighborhood median income, employment status, housing type
- Clinical: main diagnosis (diabetes, COPD, heart failure, hypertension), comorbidities, length of stay
- Healthcare utilization: number of emergency visits, 30-day readmissions, primary care follow-up

**Potential applications** :
- Predictive model for avoidable hospitalizations
- Dashboard of territorial health inequalities

---

### Question 2 : Complications cardiovasculaires chez les patients diabétiques

**Question** : Which factors predict cardiovascular complications among diabetic patients?

**Key variables** :
- Main diagnosis: type 2 diabetes
- Clinical variables: HbA1c, cholesterol, BMI, blood pressure
- Medications: insulin, statins, antihypertensives
- Outcomes: myocardial infarction, stroke, emergency hospitalization
- Behavioral factors: smoking, physical activity (if available)

**Potential applications** :
- Predictive model for cardiovascular complications
- Segmentation of diabetic patient cohorts

---

### Question 3 : Trajectoire de soins - Insuffisance cardiaque

**Question** : What is the 12-month care trajectory of patients diagnosed with heart failure after their first episode?

**Key variables** :
- Diagnosis: heart failure
- Admissions: admission and readmission dates, emergency visits
- Medications: diuretics, ACE inhibitors, beta-blockers
- Sociodemographic variables: age, sex
- Outcomes: death, prolonged hospitalization

**Potential applications** :
- Patient pathway and care trajectory analysis
- Identification of critical intervention points in heart failure management

---

### Question 4 : Perte d'autonomie chez les personnes âgées

**Question** : Which clinical and social factors predict loss of autonomy at hospital discharge among older adults?

**Key variables** :
- Age ≥ 65 years, sex, frailty score (or derived indicator)
- Diagnoses: falls, fractures, depression, dementia
- Hospital stay: length of stay, type of care received (occupational therapy, rehabilitation)/medical unit
- Outcome: Discharge destination: home, long-term care, rehabilitation center
- Readmissions: within 30 days

**Potential applications** :
- Clinical triage tool for post-discharge risk management
- Geriatric frailty and discharge planning dashboard

---

### Question 5 : Polymédication et réadmission

**Question** : Do polypharmacy patients have a higher risk of hospital readmission?

**Key variables** :
- Medication count: number of prescribed drugs (>5)
- Main chronic diagnoses
- Age, sex, length of hospital stay
- Readmissions: 30-day and 90-day
- Frailty and comorbidity indices (number/amount of comorbidity)

**Potential applications** :
- Modeling readmission risk associated with polypharmacy
- Targeted deprescription and medication optimization strategies

---

### Question 6 : Transparence des données synthétiques

**Question** : How can transparency and traceability be ensured for synthetic datasets used in clinical research?

**Key variables** :
- Metadata: dataset source, generation method (MDClone), creation date
- Anonymization level, data access license, update frequency
- Usage indicators: number of queries, users, research theme
- Synthetic data properties: structure, distribution, correlations

**Potential applications** :
- Prototype of a synthetic data transparency registry
- Governance framework for responsible research data use

---

### Question 7 : Indicateurs de santé respectueux des principes OCAP

**Question** : How can health indicators be developed that respect OCAP principles (Ownership, Control, Access, Possession)?

**Key variables** :
- Aggregated data by region or community (synthetic)
- Health indicators: screening, chronic diseases, vaccination, hospitalizations
- Social variables: housing, employment, geographic isolation, access to care
- Metadata: simulated consent, source, aggregation method

**Potential applications** :
- Participatory governance dashboard for Indigenous health data
- Simulation tool for assessing OCAP-based governance models

---

### Question 8 : Vagues de chaleur et hospitalisations

**Question** : Do summer heat waves increase the risk of hospitalizations for respiratory and cardiovascular diseases?

**Key variables** :
- Dates: admission and discharge dates
- Diagnoses: COPD, asthma, myocardial infarction, heart failure +more (dehydration)
- Environmental data: daily temperature, humidex, air quality index (AQI)
- Demographics: postal code, age, sex

**Potential applications** :
- Time-series analysis of heat-related health effects
- Climate–health dashboard for the Montréal region

---

### Question 9 : Pollution atmosphérique et MPOC

**Question** : Are high air pollution days associated with increased hospital admissions for COPD among older adults?

**Key variables** :
- Age ≥ 65 years, sex, postal code
- Diagnosis: COPD, chronic bronchitis, asthma
- Dates: admission date, length of stay
- Environmental: air quality index (AQI), mean temperature (potential linkage with CANUE dataset)

**Potential applications** :
- Correlational study on pollution and hospitalizations
- Prototype of an environmental health surveillance tool

---

### Question 10 : Défavorisation et réadmissions

**Question** : Is there a relationship between material deprivation and the frequency of 30-day hospital readmissions?

**Key variables** :
- Demographics: age, sex, postal code (linked to deprivation index)
- Admissions: primary diagnosis, admission and discharge dates
- Readmissions: 30- and 90-day frequency
- Contextual: urban/rural status, access to family physician

**Potential applications** :
- Geospatial visualization of readmission patterns
- Analysis of readmissions across the social gradient

