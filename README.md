# <center>Projet 7 : KNN </center>
Dernière mise à jour : 02/03/22
---

## Contenu :
- 1 notebook contenant le script du projet 
- 1 Rapport projet détaillant la conception du csv
- 1 le csv qui constitue notre dataframe
- 1 Rapport projet détaillant le script

---

##  Contexte du projet
Cet atelier a pour objectif de vous initier aux techniques de classification supervisé sous Python, plus précisément, nous allons manipuler le classifieur KNN, autrement dit : K plus proche voisin.

​

**Dans cet atelier, nous appliquons la classification pour prédire comment une personne gère son stress.**

​

##  Challenges

Collection d’une base de données.
Analyse, prétraitement et visualisation des données.
Préparation des données pour l’apprentissage.
Conception d’un modèle KNN.
Choix de la meilleure configuration pour le modèle KNN.
Vérification de l’efficacité de ce modèle à des nouvelles données.
Intégration de ce modèle dans l’application de test de personnalité.
​

## Phases de l’Atelier

​

## Partie 1 : Base de données, Analyse, Prétraitement et Préparation

​

Un dossier nommé « Run_Questionnaire » vous sera transmis, vous êtes censés à comprendre et maitriser le contenu et le fonctionnement de ce dossier (Votre fiche de lecture doit être notée dans le compte rendu final).

​

Exécutez le Notebook « Run.ipynb » pour collecter votre DataSet.

---

## Instruction

Chacun exécutera 10 fois le Notebook (ne pas trop concentrer sur les questions, et changer vos réponses à chaque fois). Faites attention, il y a des réponses par a, b ou c et d’autre par 1, 2 ou 3.
Pour traiter tous les cas possibles, vous êtes obligés de mettre des réponses erronées (hors proposition, exemple de réponse : w ou h ou 9 ou pas de réponse carrément).
Codez un script python qui permet de regrouper les DataSets de chacun en une seule DataSet.
​

Appliquez les traitements nécessaires pour préparer la DataSet en utilisant Numpy et Pandas, (vous pouvez trouver un référentiel sur ressource) (présenter votre pipeline dans le compte rendu). NB. Le résultat de classification dépond essentiellement de la qualité du prétraitement.

​

## Partie 2 : Développement et entraînement d’un modèle KNN

​

La technique de classification KNN est considérée comme la technique la plus simple pour appliquer la classification supervisée, tout simplement, une nouvelle donnée de test sera classée comme la majorité de ses voisins (la distance la plus proche). À la suite de votre recherche sur le principe de KNN, nous développons notre modèle KNN. Pour cela :

​

## KNN From Scratch

Préparez une fonction permettant de calculer les 3 différentes distances : Euclidean, Manhattan et Minkowski, (def distance(metric=’ Euclidean’, **kargs)).
Codez l’algorithme de KNN sous forme une fonction (def KNN(Data_Test, Data_Train, Label_Train, k=1, **kargs)) qui :
Calcul la distance entre Data de test et Data d’apprentissage.
Trouve la/les distances plus proche de « k » voisins.
Classe Data de test selon la classe majoritaire de « k » voisins.
Retourne la classe de Data Test.
Réalisez des expérimentations en variant la distance et le nombre de « k ».
Calculez les performances (exemple : Acc) et tracez la courbe de performance de chaque expérimentation. (Les résultats avec interprétation/argumentation doivent figurer dans le notebook comme dans le compte rendu).
​

## KNN Sklearn

La bibliothèque Sklearn propose un panel des techniques de classification, y compris le KNN.

Dans cette étape, vous êtes orientés vers la classe « sklearn.neighbors » pour maitriser les paramètres et les options possibles.
Vous êtes censés à préparer un modèle performant pour notre application tout en respectant les consignes de la conception d’un modèle IA (Data préparée, K-fold validation, hyperparamètre, Gridsearch). (N’oubliez pas de présenter une comparaison entre KNN From Scratch et KNN Sklearn dans le compte rendu).
​

## Partie 3 : Mettre en place la solution dans l’application de test de personnalité

​

Utilisez la fonction « joblib » pour enregistrer votre modèle, une fois vous avez préparé votre meilleur modèle de classification Faites intégrer cette solution à l’Application

​

Test de Personnalité et adapter l’application pour comparer le résultat avec et sans IA.
