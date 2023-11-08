# STRUCTURE-DE-DONNEE

Dans ce checkpoint nous avons 2 problèmes à résourdre. Nous avons donc prevu le faire en des fichiers separés
le fichier problème1.algo traite le problème 1 entièrement

dans ce problème 1

il nous est demandé de trouvez la somme de tous les éléments présents dans l’un ou l’autre des ensembles donnés.
c'est à dire des éléments distincts qui ne doivent pas se trouver dans les 2 ensembles à la fois

pour résourdre nous allons utiliser 2 tableaux differents qui vont recevoir chacun un ensemble. les éléments de chaque ensemble sont des entiers
nous allons utiliser les entiers i et j comme des compteur pour parcourir les tableaux
nous allons utiliser la variable tp comme variable tampon qui va recevoir les éléments d'un tableau qui seront comparés à tour de role à tous les éléments du second tableau

nous allons demander à l'utilsateur de definir pour chaque ensemble le nombre d'élément ce nombre sera affecté à la variable k qui permettra de 
determiner la fin du parcours de chaque tableau

une fois que les tableau ont été dimensionnés et rempli par l'utilisateur nous commençons donc la vérification proprement dite
pour le faire nous parcourons le premier tableau grace au compteur i et pour chaque élément que nous prenons et affectons à la variable tampon nous comparons cet element à tous les autres éléments du second tableau en le parcourant également grace au compteur j

Si pendant le parcours du second tableau nous trouvons une égalité d'élement nous arretons et nous passons à l'élément suivant du premier tableau
sinon nous parcourons entièrement le second tableau et si nous ne trouvons pas d'égalité nous aditionnons ce élément à somme totale. et ce jusqu'a parcourir entièrement le premier tableau

une fois le premier tableau parcouru nous inversons les tableau(ve debiyn) et cette fois nous comparons les éléments de second tableau aux éléments du premier en suivant la même demarche.  

a la fin nous avons la somme de tous les éléments distincts dans la variable som

problème 2

2 fichier pour le problème 2
le premier fichier problème2.algo traite la procedure de calcul du procedure scalaire et l'appel de cette procedure danns une lagorithme
denommé produit_scalaire

les vecteurs sont des tableaux qui contiennent les dimensions de chaque vecteur

pour calculer le produit scalaire nous avons besoin de 2 vecteurs de même dimension donc des tableaux de même taille nommé v1 et v2
la dimension des vecteurs est recupereée à partir de la variable n qui est un entier 

à partir de ces  parametres nous pouvons donc appliquer la formule de calcul du produit scalaire qui est la somme des produit de dimension de chaque vecteur par exemple pour u(a,b) et v(c,d) le produit scalaire sera a*c + b*d

pour verifier que les 2 vecteurs sont orthogonaux dans l'algorithme nous faisons appel à la procedure en lui passant les parametres (les 2 vecteurs et leur dimension) ensuite le resultat obtenu est comparé à 0. s'il est égale à 0 alors les 2 vecteurs sont orthogonaux sinon ils ne le sont pas. 
nous passons les parametres par reference ainsi ps sera le resultat du calcul que nous recuperons dans la variable ps et  qui sera utilisé pour faire la comparaison

Dans le ficier problème2bis.algo nous avons remplacé la procedure par une fonction en gardant le même principe. ici la fonction retourne directement le produit scalaire ps et nous l'utilsons pour faire le calcul sans avoir de l'affecter à une quelconque variable



