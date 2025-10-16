# 📊 RAPPORT D'ANALYSE DE LA CRIMINALITÉ À LOS ANGELES
**Période d'étude : 2020 - 2025 (octobre)**  
**Dataset : 1 000 000 lignes | 28 variables**
**Source :** *https://data.lacity.org/d/2nrs-mtv8*   
**Date du rapport : Octobre 2025**

---

## 🎯 RESUME EXECUTIF

### Vue d'ensemble
Cette analyse porte sur 1 million d'incidents criminels enregistrés à Los Angeles sur 5 ans. L'étude révèle des tendances encourageantes avec une **baisse progressive de la criminalité depuis 2022**, après un pic post-pandémie.

### Insights clés
- **📉 Tendance positive** : Criminalité en baisse continue depuis 2022, atteignant son plus bas niveau en 2025
- **🎯 Crime n°1** : Vol de véhicules (11.46% des crimes)
- **🕐 Heure critique** : Pic à 12h en journée, 22h la nuit
- **📍 Zone à risque** : Central (taux le plus élevé)
- **👥 Population vulnérable** : Hommes 26-35 ans, origine Hispanic/Latin/Mexican

### Recommandations stratégiques
1. Renforcer la surveillance dans la zone Central
2. Intensifier les patrouilles entre 12h-18h et 22h-00h
3. Campagnes de prévention ciblées sur le vol de véhicules
4. Programmes de sécurité pour les 26-44 ans

---

## 📋 TABLE DES MATIÈRES
1. [Contexte et Objectifs](#contexte)
2. [Analyse Exploratoire](#analyse)
3. [Insights Détaillés](#insights)
4. [Recommandations](#recommandations)
5. [Annexes Techniques](#annexes)

---

## 1 CONTEXTE ET OBJECTIFS {#contexte}

### Objectif principal
Analyser la criminalité à Los Angeles pour fournir aux décideurs des insights exploitables basés sur des données probantes, permettant d'optimiser l'allocation des ressources policières et les politiques de prévention.

### Questions de recherche
1. Comment évolue la criminalité à Los Angeles depuis 2020 ?
2. Quels sont les patterns temporels (heures, jours, mois) ?
3. Quelles zones géographiques nécessitent une attention prioritaire ?
4. Quels profils de victimes sont les plus vulnérables ?
5. Quels types de crimes dominent le paysage criminel ?

### Source des données
- **Origine** : Los Angeles Police Department (LAPD)
- **Période** : 2020-2025 (mise à jour : 1er octobre 2025)
- **Volume** : 1 000 000 incidents
- **Granularité** : Incident individuel avec localisation, timing, profil victime

---

## 2 ANALYSE EXPLORATOIRE {#analyse}

### 2.1 Évolution temporelle globale

#### Tendance annuelle (2020-2025)

**Observations**
- **2020** : Niveau de référence post-confinement
- **2021-2022** : Augmentation progressive (+15% environ)
- **2022** : **PIC MAXIMAL** sur la période
- **2023-2024** : Décroissance constante
- **2025** : Niveau le plus bas (données jusqu'à octobre)

**Interprétation**
La courbe suit un pattern post-crise typique : reprise d'activité criminelle après les restrictions COVID, puis retour à la normale avec amélioration. La baisse continue depuis 2022 suggère l'efficacité croissante des politiques de sécurité.

#### Saisonnalité mensuelle

**Mois le plus dangereux sur 5 ans** : **Janvier (92 701 crimes)**

**Patterns par année**
- **2020** : Pic en janvier (effet post-fêtes)
- **2021** : Octobre élevé, stabilité juillet-décembre
- **2022** : Mai critique, plateau mars-décembre
- **2023** : Octobre, cohérence juillet-janvier
- **2024** : Janvier, décroissance graduelle annuelle
- **2025** : Données incomplètes (éviter conclusions)

**Hypothèses explicatives**
- **Janvier** : Post-fêtes, vulnérabilité accrue, augmentation des déplacements
- **Variations annuelles** : Influences météo, événements locaux, changements de politiques

### 2.2 Patterns quotidiens et hebdomadaires

#### Distribution horaire (24h)

**Heure la plus dangereuse** : **12h (midi)** - pic journalier  
**Heure la plus sûre** : **5h (matin)** - creux minimal

**Dynamique journalière**
- 00h-05h : Décroissance continue (activité minimale)
- 05h-12h : Croissance forte (réveil de la ville)
- 12h : **PIC ABSOLU**
- 12h-15h : Maintien élevé
- 15h-18h : Plateau avant second pic (18h vol de véhicules)
- 18h-22h : Niveau soutenu
- 22h-00h : Décroissance progressive

#### Criminalité nocturne (22h-04h)

**Part de la criminalité totale** : **21.44%**  
**Heure critique la nuit** : **22h**

**Pattern nocturne**
- 22h : Maximum (début de soirée)
- 22h-00h : Décroissance rapide
- 00h-04h : Niveau bas et stable
- 04h-05h : Minimum absolu

#### Distribution hebdomadaire

**Semaine vs Weekend**
- **Semaine** : 71.43% des crimes
- **Weekend** : 28.57% des crimes

**Ratio** : 2.5:1 en faveur de la semaine

**Interprétation**  
La criminalité suit l'activité économique : plus de population en déplacement, plus de cibles, plus d'opportunités. Le weekend voit une concentration résidentielle et moins d'activité commerciale.

---

## 3 INSIGHTS DÉTAILLÉS {#insights}

### 3.1 Profils des victimes

#### Distribution par sexe

| Sexe | Part des victimes | Observations |
|------|-------------------|--------------|
| **Hommes** | **40.19%** | Population la plus vulnérable |
| Femmes | 35.68% | Légèrement moins exposées |
| Non renseigné | 24.13% | Absence de victime humaine identifiée |

**Analyse**  
L'écart hommes-femmes (+4.5 points) est statistiquement significatif. Les hommes sont plus exposés, probablement en raison de comportements à risque accrus et d'une plus grande mobilité urbaine.

#### Distribution par âge

**Tranche la plus vulnérable** : **26-35 ans (18.52%)**

| Tranche d'âge | Part | Profil |
|---------------|------|--------|
| 0-17 ans | 2.55% | Mineurs (très protégés) |
| 18-25 ans | 15.12% | Jeunes adultes |
| **26-35 ans** | **18.52%** | **Adultes actifs** |
| 36-44 ans | 16.87% | Adultes établis |
| 45-54 ans | 13.24% | Adultes matures |
| 55-64 ans | 9.18% | Pré-retraités |
| 65+ ans | 5.52% | Séniors (moins exposés) |

**Interprétation**  
La courbe suit une distribution normale décalée vers la gauche : pic dans la vie active (mobilité maximale, possession de biens), décroissance avec l'âge (mobilité réduite, prudence accrue).

#### Distribution par origine ethnique

**Top 3 des populations vulnérables**

1. **Hispanic/Latin/Mexican** : **29.5%**
2. **White (Blancs)** : **20.0%**
3. **Black (Noirs)** : **13.5%**

**Autres origines** : 23.0%  
**Non renseigné (NO VICTIM)** : 14.0%

**Contexte démographique**  
Cette distribution reflète partiellement la composition démographique de LA (forte population hispanique). Cependant, une analyse per capita serait nécessaire pour identifier une sur-représentation réelle.

### 3.2 Analyse géographique

#### Zones à haut risque

**Zone la plus dangereuse** : **Central**

**Top 5 des zones critiques**
1. Central
2. 77th Street
3. Pacific
4. Southwest
5. Hollywood

**Zone la plus sûre** : **Foothill**

**Analyse spatiale**  
Central concentre probablement le centre-ville avec forte densité commerciale, population flottante élevée, et concentration d'opportunités criminelles. Foothill, zone périphérique résidentielle, bénéficie d'une cohésion sociale plus forte.

### 3.3 Typologie criminelle

#### Top 5 des crimes

| Rang | Code | Type de crime | Part | Insights |
|------|------|---------------|------|----------|
| **1** | **510** | **Vol de véhicules** | **11.46%** | Crime dominant |
| 2 | 624 | Violence physique légère | 7.45% | Conflits interpersonnels |
| 3 | - | Cambriolage de véhicule | 6.32% | Cible : biens dans véhicules |
| 4 | - | Usurpation d'identité | 6.22% | Cybercriminalité croissante |
| 5 | - | Vandalisme | 6.08% | Dégradations |

#### Focus : Vol de véhicules (Crime n°1)

**Pattern horaire spécifique**
- **Premier pic** : 12h (midi)
- **Montée en flèche** : 16h-18h
- **Pic maximal** : 18h
- **Plateau** : 18h-23h
- **Chute** : 00h

**Profil des victimes**  
Tranche d'âge 26-44 ans majoritairement touchée (propriétaires de véhicules actifs)

**Hypothèses**
- 18h = fin de journée de travail, véhicules stationnés, opportunité maximale
- Nuit = risque élevé maintenu (véhicules sans surveillance)
- 00h = patrouilles nocturnes, criminels rentrent

#### Focus : Violence physique légère (Crime n°2)

**Pattern horaire spécifique**
- **Progression graduelle** : 5h-15h
- **Pic** : 15h (après-midi)
- Corrélation avec activité urbaine et consommation d'alcool

**Interprétation**  
Les violences légères suivent l'activité sociale : interactions accrues = risque de conflits accru. Le pic à 15h suggère des altercations en milieu de journée (commerces, transports).

### 3.4 Moyens utilisés

**Arme la plus utilisée** : **AUCUNE (violence physique)**

**Distribution des armes**
- **Pas d'arme (violence physique)** : Majorité écrasante
- Armes de poing : ~2%
- Pistolets semi-automatiques : ~2%
- Autres : Minoritaire

**Implication**  
La criminalité à LA est majoritairement non-armée. Les crimes violents avec armes à feu restent une minorité, contrairement à la perception médiatique.

---

## 4 RECOMMANDATIONS STRATÉGIQUES {#recommandations}

### 4.1 Allocation des ressources policières

#### Priorisation temporelle

**Heures critiques à renforcer**
- **12h-13h** : Patrouilles intensifiées (pic global)
- **16h-23h** : Surveillance accrue véhicules (vol maximal)
- **22h-00h** : Présence nocturne renforcée

**Optimisation de planning**
- Réduction des effectifs 3h-6h (période calme)
- Redéploiement vers créneaux critiques

#### Priorisation géographique

**Zones prioritaires (ordre décroissant)**
1. **Central** : Déploiement maximal, patrouilles continues
2-5. Zones intermédiaires : Présence modulée
...
N. **Foothill** : Maintien présence minimale

**Stratégie spatiale**
- Quadrillage renforcé dans Central (patrouilles + caméras + éclairage)
- Unités mobiles inter-zones pour flexibilité

### 4.2 Prévention ciblée

#### Programme anti-vol de véhicules

**Axes d'action**
1. **Campagne de sensibilisation** : "Protégez votre véhicule 16h-00h"
2. **Infrastructures** : Parkings sécurisés, éclairage public renforcé
3. **Technologie** : Incitation à l'installation de traceurs GPS
4. **Législation** : Durcissement des peines pour récidivistes

**Cible** : Propriétaires 26-44 ans (segments marketing digital)

#### Prévention des violences légères

**Axes d'action**
1. **Médiation** : Programmes de résolution de conflits dans espaces publics
2. **Formation** : Sensibilisation commerçants/transport à la désescalade
3. **Environnement** : Aménagements urbains anti-conflit (signalétique, espaces)

### 4.3 Politiques sociales

#### Protection des populations vulnérables

**Cible** : Hispanic/Latin/Mexican (29.5% victimes)

**Actions**
1. **Communication multilingue** : Matériel de prévention en espagnol
2. **Partenariats communautaires** : Associations locales
3. **Accessibilité** : Points d'accueil police dans quartiers concernés

**Cible** : Hommes 26-35 ans

**Actions**
1. **Prévention comportementale** : Campagnes sur les risques
2. **Programmes de mentorat** : Jeunes à risque

### 4.4 Suivi et évaluation

**Indicateurs clés de performance (KPI)**

| Indicateur | Fréquence | Cible 2026 |
|------------|-----------|------------|
| Nombre total de crimes | Mensuel | -10% vs 2025 |
| Vols de véhicules | Hebdomadaire | -15% |
| Crimes zone Central | Mensuel | -20% |
| Taux de résolution | Trimestriel | +10% |

**Révision stratégique** : Trimestrielle avec ajustement des ressources

---

## 5 ANNEXES TECHNIQUES {#annexes}

### A. Limites de l'étude

**Limites méthodologiques**
1. **Année 2025 incomplète** : Données jusqu'à octobre uniquement
2. **Données manquantes** : 14% victimes non identifiées
3. **Biais de signalement** : Crimes non rapportés à la police exclus
4. **Géolocalisation** : Adresses approximatives (protection vie privée)

**Limites d'interprétation**
1. **Causalité** : Les corrélations observées ne prouvent pas de causalité
2. **Généralisation** : Résultats spécifiques à Los Angeles
3. **Évolution temporelle** : Contextes 2020 (COVID) vs 2025 différents

### B. Pistes d'amélioration futures

**Enrichissement des données**
1. Croisement avec données socio-économiques (pauvreté, chômage)
2. Intégration données météo (influence température/crime)
3. Données démographiques per capita (calcul taux réels)

**Analyses avancées**
1. Modélisation prédictive (Machine Learning)
2. Analyse de clustering géospatial (hotspots)
3. Analyse de réseaux criminels (récidive)

---

## CONTACT ET AUTEUR

**Analyste** : Akandé Philippe ABIODOUN 
**Date de production** : Octobre 2025  
**Outils** : Python 3.x, Pandas, Matplotlib, Seaborn, Jupyter Notebook  
**Accès aux données** :
    - *https://drive.google.com/file/d/1_I9GbgNx-I01JH1CiQ9mLnVbcOEIswJc/view?usp=sharing*
    - *https://drive.google.com/file/d/19TB3S3rxFykB8dqfSQ3iV1tjGnAL2Gbk/view?usp=sharing*
**Notebooks** : *https://github.com/vrmelox/datanip*

---

## 📚 RÉFÉRENCES

1. Los Angeles Police Department (LAPD) - Crime Data 2020-2025
2. Documentation Python : Pandas, Matplotlib, Seaborn
3. Littérature académique sur patterns criminels urbains
4. Best practices nettoyage de données (Missing Data Theory)

---

*Ce rapport a été produit dans le cadre d'une analyse exploratoire approfondie visant à éclairer les décisions stratégiques en matière de sécurité publique à Los Angeles.*