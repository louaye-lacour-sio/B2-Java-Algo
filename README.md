# <ins>Java TD - Collections et algorithmes - Lacour Louaye</ins>

## 1- Comparaisons

## B2GNSAlgo11

### 1.1- Joueur
1.1) Création du projet B2GNSAlgo11 avec son package et importation des classes


1.2) Lors de l'évaluation de l'expression jr1 == jr2 , le résultat obtenu indique une différence entre les 2 variables parce que ce ne sont pas les mêmes objets qu'elles référencent.

1.3) Lors de l'évaluation de l'expession jr1.equals(jr2), on nous indique une différence entre jr1 et jr2 et cela est du au fait que la méthode equals(Object obj) renvoie True si et seulement si les 2 éléments référencent le même objet mais puisqu'il s'agit de 2 objets différents c'est False.

## B2GNSAlgo12
### 1.2- Numéro de joueur en tant que critère de comparaison
1.4) Création du projet B2GNSAlgo11 avec son package et importation des classes

1.5) Implémentation de la méthode equals surchargée dans la Classe Joueur :
```	public boolean equals(Joueur autre) {
		System.out.println("[Joueur::equals(Joueur):boolean]");
		if (this.numero == autre.numero){
			return true;
		}
		else {
			return false;
		}
	}```

1.6) Une fois encore, jr1 == jr2 montre une différence car les variables ne référencent pas les mêmes objets.

1.7.1) Après la compilation et l'exécution du programme, le résultat obtenu est True ("les deux joueurs sont identiques") car la méthode equals surchargée compare l'attribut numero des objets référencés par jr1 et jr2.

## B2GNSAlgo13
### 1.3- Nombre de victoires en tant que critère de comparaison

1.7.2) Création du projet B2GNSAlgo11 avec son package et importation des classes

1.8) Implémentation de compareTo(Joueur) dans la Classe Joueur :
```
d
```

1.9) Après avoir effectué une vérification Watson (Joueur 2) est meilleur que Parker (Joueur 1) et lorsque l'on vérifie les attributs des 2 objets le Joueur 2 à effectivement plus de victoires que le Joueur 1

## 2- Comparaisons et relations d'ordre

## B2GNSAlgo21
### 2.1- Collection d'objets dont la classe implémente l'interface Comparable<T>