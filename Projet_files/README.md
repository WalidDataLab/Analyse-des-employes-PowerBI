# 📊 Rapport d'analyse RH – Power BI

> **Note importante** : Les données utilisées dans ce projet sont **des données de test fictives** et ne reflètent pas une réalité organisationnelle. Elles ont été conçues uniquement à des fins d'apprentissage et d'expérimentation. Cependant, **le projet est entièrement fonctionnel** : en remplaçant le fichier source par une base de données réelle, l'ensemble du tableau de bord se met à jour automatiquement et peut être exploité immédiatement en production.

---

## 🗂️ Structure du rapport

Le rapport Power BI est composé de **trois pages principales** :

| Page | Titre | Contenu |
|------|-------|---------|
| 1 | Navigation & Présentation | Page d'accueil et menu de navigation |
| 2 | Rapport du personnel | Vue d'ensemble RH |
| 3 | Analyse RH & Salaires | Rémunération & performance |

## 🧾 1. Présentation
![SCREENSHOOT](Présentation.PNG)

---

## 🧾 2. Rapport du personnel

![SCREENSHOOT](https://github.com/WalidDataLab/Analyse-des-employ-s/blob/main/Rapport%20du%20personnel.PNG)

### 🔎 Présentation générale

Ce tableau de bord, réalisé avec Power BI, permet d'analyser les ressources humaines de l'entreprise à travers plusieurs indicateurs clés tels que le nombre d'employés, la masse salariale et la répartition par département, pays et genre.

### 🎛️ Filtres disponibles

Le rapport contient un menu de sélection des pays :
- 🇪🇬 Égypte
- 🇱🇧 Liban
- 🇸🇦 Arabie Saoudite
- 🇸🇾 Syrie
- 🇦🇪 Émirats Arabes Unis

Ces filtres permettent de :
- Analyser les données par pays
- Comparer les performances entre différents marchés
- Adapter les décisions stratégiques selon chaque région

### 📈 Analyse & insights

**🟢 Égypte — Marché stratégique principal**
- Plus grand nombre d'employés
- Masse salariale la plus élevée

> Cela en fait un marché stratégique qui peut être développé pour augmenter la production, ou optimisé pour réduire les coûts.
![SCREENSHOOT](https://github.com/WalidDataLab/Analyse-des-employ-s/blob/main/Egypt.PNG)



**🔴 Liban — Marché atypique**
- Plus faible nombre d'employés
- Un seul employé recensé dans le département Manufacturing

> Cela suggère que l'entreprise a récemment commencé ses activités dans ce pays, ou qu'une situation particulière affecte ce marché.
![SCREENSHOOT](lebanon.PNG)

**📉 Baisse des effectifs (2019–2020)**

Une diminution du nombre d'employés est observée entre 2019 et 2020. En l'absence de données sur les revenus, il est difficile de déterminer si cette baisse est due à des difficultés financières ou à des départs volontaires.

---

## 🧾 3. Analyse RH & Salaires
![SCREENSHOOT](https://github.com/WalidDataLab/Analyse-des-employ-s/blob/main/Analyse%20RH%20%26%20Salaires.PNG)


### 💰 Présentation générale

Cette page se concentre sur l'analyse des salaires, des performances et de la répartition des effectifs selon le genre, le département et le pays.

### 📊 Analyse & insights

**⚖️ Déséquilibre hommes / femmes**

Il existe une différence notable entre le nombre d'hommes et de femmes dans l'entreprise, ce qui reflète un manque d'équilibre en termes d'égalité professionnelle.

> Recommandation : renforcer le recrutement féminin pour atteindre une meilleure parité.

**✅ Équité salariale**

L'écart entre les salaires moyens des hommes et des femmes est faible, ce qui indique une certaine équité salariale au sein de l'organisation.

**🏢 Salaires par département**
- Le département **HR** affiche le salaire moyen le plus élevé au niveau global
- En **Arabie Saoudite**, c'est le département **Facilities/Engineering** qui présente les salaires les plus élevés (2 999 $/mois en moyenne)

![SCREENSHOOT](https://github.com/WalidDataLab/Analyse-des-employ-s/blob/main/Saudi%20arabia.PNG)

**📊 Relation salaire / performance par pays**

| Pays | Salaire moyen | Performance | Analyse |
|------|--------------|-------------|---------|
| Arabie Saoudite | Modéré | Élevée | Meilleur rendement |
| Liban | Plus faible | Faible | Coût / performance déséquilibré |
| Égypte | Le plus élevé | — | Marché à fort potentiel |

**🔎 Cas particulier du Liban**

Bien que le Liban affiche le salaire moyen le plus faible, ses scores de performance (Job Rate) sont également les plus bas. Rapporté au faible nombre d'employés, ce constat soulève plusieurs hypothèses :

- Les données disponibles pourraient être **insuffisantes ou non représentatives**, compte tenu du très petit effectif
- Il est possible que l'activité concernée ait été **acquise récemment auprès d'une entité en difficulté**, et que l'entreprise soit en phase de restructuration
- Le nombre d'employés enregistré est **anormalement bas pour un projet opérationnel**, ce qui renforce l'idée d'un démarrage récent ou d'une reprise d'activité

> Dans tous les cas, des données complémentaires (revenus, historique, contexte d'acquisition) seraient nécessaires pour valider l'une de ces hypothèses.

---

## ✅ Conclusion générale

Ce tableau de bord Power BI permet d'identifier des opportunités d'optimisation des ressources humaines, d'améliorer la répartition des effectifs et de mieux contrôler les coûts tout en maintenant un bon niveau de performance.

Les principaux enseignements sont :

- 📍 L'**Égypte** est le marché le plus mature et le plus stratégique
- 🔍 Le **Liban** nécessite une analyse approfondie et des données complémentaires avant toute décision
- ⚖️ La **parité hommes/femmes** mérite d'être améliorée
- 💡 La **performance n'est pas corrélée au salaire** — un levier d'optimisation RH à explorer
---

## 🛠️ Stack technique

| Outil | Usage |
|-------|-------|
| Power BI Desktop | Visualisation & tableaux de bord |
| Microsoft Excel (.xlsx) | Source de données |
| DAX | Mesures et indicateurs calculés |

---

## 📁 Structure des fichiers

```
📦 HR-PowerBI-Report
 ┣ 📊 Employees.xlsx        ← Fichier source des données
 ┣ 📈 RH_Dashboard.pbix     ← Rapport Power BI (3 pages)
 ┗ 📄 README.md             ← Documentation du projet
```

---

## 🚀 Comment utiliser ce projet

1. **Cloner** ce dépôt
2. **Ouvrir** le fichier `RH_Dashboard.pbix` avec Power BI Desktop
3. **Remplacer** le fichier `Employees.xlsx` par vos propres données (en conservant la même structure de colonnes)
4. **Actualiser** les données dans Power BI
5. Le tableau de bord se met à jour **automatiquement**

---

## 📌 Colonnes requises dans le fichier Excel

| Colonne | Type | Description |
|---------|------|-------------|
| No | Entier | Identifiant employé |
| First Name / Last Name | Texte | Nom complet |
| Gender | Texte | Male / Female |
| Start Date | Date | Date d'embauche |
| Years | Entier | Ancienneté |
| Department | Texte | Département |
| Country | Texte | Pays |
| Center | Texte | Centre de travail |
| Monthly Salary | Entier | Salaire mensuel |
| Annual Salary | Entier | Salaire annuel |
| Job Rate | Décimal | Note de performance (1–5) |
| Sick Leaves | Entier | Jours de congés maladie |
| Unpaid Leaves | Entier | Jours de congés non payés |
| Overtime Hours | Entier | Heures supplémentaires |

---

*Projet réalisé à des fins d'apprentissage et de démonstration — données fictives.*
