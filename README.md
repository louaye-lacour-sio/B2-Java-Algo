# <ins>Java TD - Collections et algorithmes - Lacour Louaye</ins>

## 1- Comparaisons

## B2GNSAlgo11

### 1.1- Joueur
1.1) Création du projet B2GNSAlgo11 avec son package et importation des classes.


1.2) Lors de l'évaluation de l'expression jr1 == jr2 , le résultat obtenu indique une différence entre les 2 variables parce que ce ne sont pas les mêmes objets qu'elles référencent.

1.3) Lors de l'évaluation de l'expession jr1.equals(jr2), on nous indique une différence entre jr1 et jr2 et cela est du au fait que la méthode equals(Object obj) renvoie True si et seulement si les 2 éléments référencent le même objet mais puisqu'il s'agit de 2 objets différents c'est False.

## B2GNSAlgo12
### 1.2- Numéro de joueur en tant que critère de comparaison
1.4) Création du projet B2GNSAlgo12 avec son package et importation des classes.

1.5) Implémentation de la méthode equals surchargée dans la Classe Joueur :
```	
    public boolean equals(Joueur autre) {
		System.out.println("[Joueur::equals(Joueur):boolean]");
		if (this.numero == autre.numero){
			return true;
		}
		else {
			return false;
		}
	}
```

1.6) Une fois encore, jr1 == jr2 montre une différence car les variables ne référencent pas les mêmes objets.

1.7.1) Après la compilation et l'exécution du programme, le résultat obtenu est True ("les deux joueurs sont identiques") car la méthode equals surchargée compare l'attribut numero des objets référencés par jr1 et jr2.

## B2GNSAlgo13
### 1.3- Nombre de victoires en tant que critère de comparaison

1.7.2) Création du projet B2GNSAlgo13 avec son package et importation des classes.

1.8) Implémentation de compareTo(Joueur) dans la Classe Joueur :
```
    public int compareTo(Joueur autre) {
	    System.out.println("[Joueur::compareTo(Joueur):int]");
	    if (this.nbVictoires == autre.nbVictoires){
	    	return 0;
	    }
	    else if (this.nbVictoires > autre.nbVictoires){
	    	return 1;
	    }
	    else{
		    return -1;
	    }
    }
```

1.9) Après avoir effectué une vérification Watson (Joueur 2) est meilleur que Parker (Joueur 1) et lorsque l'on vérifie les attributs des 2 objets le Joueur 2 à effectivement plus de victoires que le Joueur 1

## 2- Comparaisons et relations d'ordre

## B2GNSAlgo21
### 2.1- Collection d'objets dont la classe implémente l'interface Comparable\<T\>

2.1) Création du projet B2GNSAlgo21 avec son package et importation des classes.

2.2) Utilisation de Collections.min : 
```
	System.out.println( "\nCelui qui a remporté le moins de victoires :\n" ) ;
			Joueur pireJoueur = Collections.min(joueurs);
			System.out.println(pireJoueur);
```

2.3) Utilisation de Collections.sort :
```
	System.out.println( "\nListe triée des joueurs :\n" ) ;
		Collections.sort(joueurs);
		for (Joueur joueur : joueurs) {
			System.out.println(joueur);
		}
```

## B2GNSAlgo22
### 2.2- Collection d'objets dont la class N'implément PAS l'interface Comparable\<T\>

2.4) Création du projet B2GNSAlgo22 avec son package et importation des classes.

2.5) Dans ComparateurNbVictoires : 
```
	@Override
	public int compare(Joueur o1, Joueur o2) {
		// TODO Auto-generated method stub
		return o1.getNbVictoires() - o2.getNbVictoires();
	}
```
Dans AppTrierParNbVictoires :
```
	System.out.println( "\nListe triée des joueurs :\n" ) ;
		Collections.sort(joueurs, new ComparateurNbVictoires());
		for( Joueur joueur : joueurs ) {
			System.out.println( joueur ) ;
		}

```

## 3- Recherche

## B2GNSAlgo31

3.1) Création du projet B2GNSAlgo31 avec son package et importation des classes.

3.2)

3.3) Création du projet B2GNSAlgo32 avec son package et importation des classes.

3.4)

3.5) Modification apportée :
```

```