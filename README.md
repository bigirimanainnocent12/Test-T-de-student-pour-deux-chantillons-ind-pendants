# *🎯 Objectif général*
Ce projet vise à comparer deux groupes indépendants à l’aide du test t de Student, dans deux contextes distincts :

Comparaison de poids entre Manala et Manele (brioches alsaciennes)
Évaluation de l’efficacité d’une molécule expérimentale sur une mesure physiologique
# *1. 🥐 Étude sur les brioches Manala vs Manele*

*🔍 Problématique*
Alice, récemment arrivée en Alsace, souhaite savoir s’il existe une différence de poids entre les brioches Manala et Manele.

*📦 Données*
Fichier : Man.csv
Variables : poids des brioches Manala et Manele (en grammes)
*📈 Étapes de l’analyse*
Statistiques descriptives : moyenne, écart-type, etc.
Test de normalité (Shapiro-Wilk) : vérification de la distribution normale
Visualisations : Q-Q plots, histogrammes avec courbes normales
Test de Fisher-Snedecor : comparaison des variances
Test t de Student : comparaison des moyennes
Analyses complémentaires :
Intervalle de confiance
Taille d’effet (Cohen’s d)
Bayes Factor (BF10)
Puissance du test
*✅ Conclusion*
Aucune différence significative détectée entre les poids des deux types de brioches.
Faible puissance du test → nécessité d’un échantillon plus grand pour confirmer.
# *2. 💊 Étude sur l’efficacité d’une molécule*
*🔍 Problématique*
Une entreprise pharmaceutique souhaite tester l’efficacité d’une nouvelle molécule sur une mesure physiologique.

$📦 Données*
Fichier : molecule.csv
54 patients répartis aléatoirement :
Groupe A : molécule
Groupe B : placebo
*📈 Étapes de l’analyse*
Statistiques descriptives pour chaque groupe
Test de normalité (Shapiro-Wilk) pour chaque groupe
Test de Fisher-Snedecor pour l’égalité des variances
Test t de Student unilatéral (greater) pour comparer les moyennes
Analyses complémentaires :
Intervalle de confiance
Taille d’effet (Cohen’s d)
Bayes Factor (BF10)
Puissance du test
*✅ Conclusion*
La molécule a un effet significatif et important sur la mesure physiologique.
Résultats soutenus par :
p-value très faible
Cohen’s d élevé
BF10 très fort
Puissance du test proche de 1
*🛠️ Technologies utilisées*
Python
Pandas, NumPy
Pingouin (tests statistiques)
Seaborn, Matplotlib (visualisation)
SciPy, Statsmodels
