# Feedback2 Parcours
*le 13 janvier 2023*

Félicitations pour ce parcours.
Les notions apprises lors de cette saison seront bientôt acquises.

En complément de la correction et suite à ta demande, voici un feedback pour aller plus loin. :smiley:

**Etape 1:**
L'affichage de la carte sélectionnée est fonctionnel, mais il aurait été bien d'afficher également les données de celle-ci.

**Etape 2:**
Il manque l'affichage des cartes n'étant pas associées à un élément. Cela se gère facilement en rajoutant, dans la méthode `getElements`, une condition avec une requête pour obtenir les cartes où l'élément `IS NULL` (voir la correction pour les détails).
Tu aurais également pu afficher le visuel des cartes trouvées en plus de leur nom.

**Etape 3:**
Lors de la mise en place des sessions, attention à ne pas laisser en clair le `secret` et le mettre plutôt dans les variables d'environnement (.env).
Bravo! Même si tu n'as pas pu terminer, l'ajout de cartes dans le deck fonctionne bien, leur affichage dans celui-ci aussi.
Quelques infos [ici](https://www.npmjs.com/package/express-session#user-content-secret).

Il t'a manqué un peu de temps sur ce parcours, mais je suis sûre qu'avec un délai supplémentaire tu aurais pu le finaliser facilement. :muscle:

Encore quelques conseils:
- pense à espacer chaque méthode dans tes fichiers pour plus de lisibilité du code.
- Prête également attention aux noms de tes methodes et fonctions. Par exemple `getElements` est un peu confusant, alors qu'un `getCardsByElement` est tout de suite plus clair.

Si tu as des questions complémentaires, n'hésite pas.