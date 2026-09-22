# 📊 Analyse Économétrique : Pénibilité Physique et Satisfaction au Travail

> **Projet académique (L3 Économie-Gestion)** — Étude empirique des conditions de travail et du bien-être professionnel en France à partir des données de l'enquête européenne **SRCV 2015** (Insee / Eurostat).

---

## 🚀 Contexte et Objectifs du Projet
Ce projet explore les mécanismes de la qualité de vie au travail à travers deux axes de modélisation distincts mais complémentaires :
1. **Modèle 1 (Logit Simple) :** Quels sont les facteurs socio-démographiques et le rôle du diplôme qui exposent un travailleur aux contraintes et à la **pénibilité physique** (port de charges, postures pénibles) ?
2. **Modèle 2 (Logit Ordonné) :** Comment les conditions d'exercice (pression, promotion), la santé et le parcours de vie (âge, satisfaction de vie globale) influencent-ils le niveau de **satisfaction au travail** ?

L'intégralité du traitement des données, du nettoyage et des estimations économétriques a été réalisée sous **Stata**.

---

## 🛠️ Stack Technique & Méthodologie
* **Langage & Outils :** Stata
* **Méthodes statistiques et économétriques :**
  * Statistiques descriptives univariées et bivariées (tests du Chi-2 d'indépendance).
  * **Modèle Logit Simple** (odds ratios, effets marginaux, courbes ROC et tableaux de concordance).
  * **Modèle Logit Ordonné** pour variables ordinales à plusieurs niveaux.
  * Tests de robustesse et de validation (test d'égalité des pentes de Brant).

---

## 📂 Structure et Principaux Résultats

### 1. Modèle 1 : Les déterminants de la Pénibilité Physique (Logit)
* **Variable expliquée ($Y_1$) :** Exposition fréquente ou constante à des contraintes physiques.
* **Variable d'intérêt :** Le niveau de diplôme (`ddipl`).
* **Résultats clés :** 
  * Mise en évidence d'un net effet "bouclier" du capital humain : le risque d'exposition à la pénibilité physique diminue fortement à mesure que le niveau de diplôme s'élève.
  * Les détenteurs d'un CAP/BEP ou d'un niveau inférieur au brevet affichent une probabilité significativement accrue d'occuper un emploi pénible par rapport aux diplômés du supérieur.
  * Bon pouvoir discriminant du modèle validé par une aire sous la courbe ROC de **0.7381**.

### 2. Modèle 2 : Les déterminants de la Satisfaction au Travail (Logit Ordonné)
* **Variable expliquée ($Y_2$) :** Niveau de satisfaction professionnelle mesuré sur une échelle ordonnée (Faible, Moyenne, Élevée).
* **Variable d'intérêt :** L'âge et les étapes de la carrière.
* **Résultats clés :**
  * **L'impact psychologique global :** La satisfaction de la vie personnelle (`viesatisf`) s'avère être le prédicteur le plus puissant du bien-être professionnel (le bonheur personnel "déborde" massivement sur la sphère de travail).
  * **L'effet de l'organisation :** L'absence de pression temporelle et l'existence de perspectives de promotion augmentent spectaculairement les chances d'épanouissement.
  * **Le paradoxe du salaire et du diplôme :** Une fois contrôlé par la pénibilité, la pression et les conditions de travail, le niveau de revenu brut et le diplôme perdent de leur significativité directe sur la satisfaction, redéfinissant la centralité des conditions non-pécuniaires.

---

## 👤 Auteur
* **Eric Lin** — Étudiant en Master 1 Data Sciences for Social Sciences (Université Paris Nanterre) & Licence en Économie-Gestion (Université Paris-Panthéon-Assas)
