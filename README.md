# Projet : Bootstrap & Algorithme EM

Ce projet contient deux volets principaux d’analyse statistique appliquée :

- l’étude de l’incertitude via le **bootstrap** dans un modèle de régression logistique
- l’implémentation et l’analyse de l’**algorithme EM** pour des modèles de mélanges avec censure

---

# Partie I — Bootstrap et régression logistique

## Objectif

On utilise le jeu de données `heart.csv` (Kaggle) pour expliquer la variable binaire `target`, indiquant si un patient est à risque cardiovasculaire.

## Modèle

On considère un modèle de régression logistique :

## Contributions

### 1. Intervalle de confiance bootstrap

- Mise en place d’un bootstrap non paramétrique  
- Estimation d’un intervalle de confiance à 95% pour le coefficient βAge  
- Analyse de la variabilité de l’estimateur  

### 2. Test d’hypothèse bootstrap

- Hypothèse nulle : βAge = 0  
- Construction d’un test basé sur la distribution bootstrap  
- Décision sur la significativité de l’âge  

---

# Partie II — Algorithme EM pour modèles de mélanges avec censure

## Objectif

Ce travail est basé sur l’exposé *“Estimation de modèles de mélanges en présence de censure”* (Bordes & Chauveau).

L’objectif est de comprendre et implémenter l’algorithme EM dans un cadre de données incomplètes et/ou censurées.

---

## Contenu du rapport

### 1. Contexte

Présentation du problème d’estimation dans les modèles de mélanges avec données censurées et objectifs méthodologiques.

### 2. Notations et cadre formel

- **X** : variable observée  
- **Z** : variable latente (appartenance de classe)  
- **θ** : paramètre du modèle  
- Espaces probabilistes associés  

### 3. Dérivation des formules EM

Justification rigoureuse des étapes E et M (diapo 21 de l’exposé).

### 4. Implémentation — exemple simulé 1

- Implémentation de l’algorithme EM sur données simulées (diapo 22)
- Suivi de la log-vraisemblance
- Analyse de la sensibilité aux points de départ

### 5. Application à des données réelles

- Ajustement du modèle sur un jeu de données réel
- Interprétation des résultats

### 6. Exemple simulé 2

- Implémentation sur un second exemple (diapo 31)
- Analyse de convergence
- Étude de la stabilité selon l’initialisation

### 7. Application complémentaire

- Nouvelle application sur données réelles

### 8. Conclusion

- Bilan des résultats
- Limites de l’algorithme EM
- Perspectives d’amélioration

### 9. Bibliographie

- Bordes & Chauveau
- Support de cours associé
- Littérature sur les modèles de mélanges et EM
