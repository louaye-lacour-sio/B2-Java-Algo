# <ins>Java TD - Collections et algorithmes - Lacour Louaye</ins>

## 1- Comparaisons

## B2GNSAlgo11

### 1.1- Joueur

```1.2) Lors de l'évaluation de l'expression jr1 == jr2 , le résultat obtenu indique une différence entre les 2 variables parce que ce ne sont pas les mêmes objets qu'elles référencent.```

```1.3) Lors de l'évaluation de l'expession jr1.equals(jr2), on nous indique une différence entre jr1 et jr2 et cela est du au fait que la méthode equals(Object obj) renvoie True si et seulement si les 2 éléments référencent le même objet mais puisqu'il s'agit de 2 objets différents c'est False.```

## B2GNSAlgo12
### 1.2- Numéro de joueur en tant que critère de comparaison

```1.6) Une fois encore, jr1 == jr2 montre une différence car les variables ne référencent pas les mêmes objets.```

```1.7) Après la compilation et l'exécution du programme, le résultat obtenu est True ("les deux joueurs sont identiques") car la méthode equals surchargée compare l'attribut numero des objets référencés par jr1 et jr2.```

### 1.3- Nombre de victoires en tant que critère de comparaison

