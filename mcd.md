# Retours MCD

Ton MCD est plutôt bien fait, j'ai cependant quelques modifications à te suggérer.

1. utilise plutôt des rectangles arrondis pour les relations entre les entités, ça rend le tout plus lisible.
2. Le discriminant (identifiant unique), doit être souligné pour le distinguer facilement.
3. L'email est une information qui doit être unique, donc il est mieux de l'utiliser comme discriminant.
4. Pour la relation entre `user` et `product` :
    1. Côté `user` il faut plutôt une cardinalité 0,N (un user peut liker 0 à N produits).
    2. Coté `product` il faut plutôt une cardinalité 0,N (un produit peut être liké par 0 à N users).
5. Pour la relation entre `user` et `adress` : Côté `user` il faut plutôt une cardinalité 1,N (un user doit avoir au moins une adresse mais peut en avoir plusieurs).
6. Il faudrait également rajouter une relation entre `order` et `adress` pour indiquer l'adresse de livraison de la commande :
   1. Côté `order` une cardinalité 1,1 (une commande doit avoir une et une seule adresse de livraison).
   2. Côté `adress` une cardinalité 0,N (une adresse peut être utilisée pour plusieurs commandes).

Voici en complément, des liens vers des outils pour créer tes MCD :
- [draw.io](draw.io) : un outil en ligne pour créer des MCD, qui possède également une extension VSCode.
- [mocodo](https://www.mocodo.net/) : un peu plus difficile à utiliser au début mais assez complet.
- [gitMind](https://gitmind.com/fr/) : logiciel gratuit pour créer des MCD.