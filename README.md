# Exemple de projet CGAL

## Compilation

* se rendre dans le répertoire ```build```, puis préparer la compilation avec ```cmake ..```
* compiler avec la commande ```make```

## Utilisation

Les programmes sont exutables depuis le répertoire ```build```:
```
./genre ../data/cube.off
./measures ../data/adapter.off
```

Ce qui produit, pour l'exécutable ```genre``` la sortie suivante:

```
Nombre de sommets: 8
Nombre d'arêtes: 12
Nombre de faces: 6
En supposant que le maillage contienne une unique surface sans bord, alors son genre est de 0
````

## Ajout d'un nouveau programme

Le fichier ```src/CMakeLists.txt``` est facilement adaptable pour ajouter de nouveaux exécutables, ne pas oublier de linker CGAL à l'exécutable grâce à la routine target_link_libraries.
