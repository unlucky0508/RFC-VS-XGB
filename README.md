# RFC-VS-XGB
Etude de machine learning sur la prédiction du cours des actions 

Implémentation du devoir 4

Lucca MASI MASL05080300

Problématique : comment créer un algorithme de machine learning permettant de prédire le cours des actions?

BDD : Sp500 (cour des actions global depuis le 3 Janv 19500 )

vidéo explicative : https://youtu.be/p9iXoSNGGj8

projet github : https://github.com/unlucky0508/RFC-VS-XGB

Courte explication : 

Tout d'abord on importe et prépare les données puis on les visualises pour comprendre le jeu de donnée. Ensuite on implémente une fonction de prédiction (la ou on va utiliser le modèle pour prédire les années suivantes) et de backtest (comme on utilise des données temporelles, on ne peut pas faire de validation croisée). 

1er modèle : RandomForestClassifier

On commence par déterminer les "prédicteurs" puis on appel la fonction de backtest avec notre modèle. on affiche ensuite les métrics du modèle ainsi que le temps d'éxecution pour pouvoir les comparer avec l'autre implémentation.

2eme modèle : XGBClassifier  

On commence par déterminer les "prédicteurs" puis on appel la fonction de backtest avec notre modèle. on affiche ensuite les métrics du modèle ainsi que le temps d'éxecution pour pouvoir les comparer avec l'autre implémentation.


Conclusion :

La précision des deux algorithme  est très proche. Le premier étant légèrement plus précis mais nécessitant un plus grand temps d'éxecution. Le second modèle, contrairement au premier est  bien plus rapide mais est légèrement moins précis. Dans les deux cas, la précision obtenu est approximativement 51.5% ce qui est assez faible comme résultat. En comparant cette implémentation à d'autre, on se rend compte que cette précision est assez "normal" pour ce genre d'algorithme.  Il est rare d'avoir un précision qui dépasse les 60% sur ce genre d'algorithme.
