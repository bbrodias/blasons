# Lien entre l'activité de Nim et l'informatique

On utilise ici à la fois la classification en 4 concepts (Algorithme,
Langage, Information et données, et Machine) que l'on retrouve à
plusieurs niveaux dans les programmes français, et la classification
en (six compétences de la pensée informatique)[https://csunplugged.org/en/computational-thinking/]
dues à Tim Bell et ses collègues de CS unplug.

On s'attache également à se raccrocher à des éléments de la vie de
tous les jours pour raccrocher ces concepts au vécu des participants.

## Concepts de l'informatique

### Algorithme (\*\*)
Au cours de l'activité, les participants sont amenés à trouver une méthode permettant de gagner automatiquement au jeu de Nim (lorsque l'on joue en deuxième). C'est-à-dire, les participants doivent être capables de prendre un nombre d'allumettes précis en fonction du nombre d'allumettes qui a été précédemment pris. Ainsi, il faut mettre en place une procédure de décision qui, à partir du nombre d'allumettes pris, renvoie le nombre d'allumettes à prendre. Cette procédure prend donc en entrée un nombre et en renvoie un autre. Ici, à partir du nombre n entre 1 et 3 reçu, elle renvoie le nombre 4-n. Cette procédure est en fait un algorithme. C'est-à-dire, c'est une suite d'instructions qui, en fonction d'une entrée, renvoie une sortie. La suite d'instructions de cet algorithme est assez limitée étant donné qu'il s'agit uniquement de renvoyer le résultat de l'opération 4-n. Cependant, on peut imaginer des algorithmes plus complexes, qui nécessiteraient des calculs intermédiaires plus développés. 

Une fois cet algorithme mis en place, les participants n'ont plus qu'à l'exécuter à chaque fois qu'un coup doit être joué pour connaître le nombre d'allumettes à prendre. L'algorithme mis en place doit alors permettre de gagner toutes les parties (si l'on joue en second). On peut alors se poser la question des garanties que cet algorithme donne. Peut-on prouver que cet algorithme assure la victoire au jeu de Nim ? Cela pose la question de la correction de l'algorithme : si, dans les spécifications de l'algorithme, on a que le suivre permet de gagner au jeu de Nim, prouver sa correction revient à prouver que si on l'exécute jusqu'au bout, on gagnera nécessairement au jeu de Nim.

La notion de correction des algorithmes est primordiale attendu que cela peut permettre d'assurer que des systèmes exécutant des algorithmes sensibles (atterissage d'un avion, déploiement d'un airbag, ...) vérifient des propriétés de sécurité.

### Langage (.)

### Information et Données (.)
Le jeu de Nim fait partie de la classe des jeux à information parfaite : les jeux où les joueurs connaiseent tout ce qui s'est passé au moment de prendre leur décision. Le jeu d'échecs et le jeu de go sont deux exemples de jeux à information parfaite. Résoudre ces jeux peut théoriquement se faire de la même manière que le jeu Nim : à partir de positions gagnantes pour l'un ou l'autre joueur, on établit successivement quelles positions sont gagnantes pour quel joueur en remonattn selon les coups qui ont pu être joués pour remonter jusqu'à la position intiale. Cependant pour des jeux comme le jeu d'échecs ou le jeu de go, il est beaucoup (beaucoup !) plus complexe de considérer toutes les positions étant donné le nombre collosalle de possiblités avec seulement quelques coups  (au delà de la légère difficulté de prendre en compte la partie nulle). 

Il existe également des jeux à information imparfaite, sur lesquels la décision des joueurs se fait alors que certains éléments leur sont inconnus, c'est par exemple le cas du poker. 

### Machine (.)

## Compétences de la pensée informatique

### Abstraction/Modélisation (.)

### Décomposition (\*)
Cette notion et la suivante (généralisation et motifs) sont très liées pour cette activité et seront donc discuter en même temps. Pour mettre en place l'algorithme de résolution, il faut décomposer le problème en problèmes plus simples. Inititalement, il faut résoudre le problème avec 4 allumettes, puis résoudre avec 8 alluemettes, etc... Il faut pouvoir généraliser aux cas avec un nombre arbitraire d'allumettes (toujours multiple de 4). Cela nécessite donc de repérer le motif des 4 allumettes à partir de la décomposition en problème plus élémentaires.

### Généralisation et motifs (\*)
Voir Décomposition.

### Évaluation ()

### Pensée algorithmique (\*\*)



### Logique (\*)
Les participants sont censés avoir aboutit à la stratégie suivante : jusqu'à la fin du jeux, si mon adversaire prend 1 allumette, je dois en prendre 3, s'il en prend 2, je dois en prendre 2 et s'il en prend 3 je dois en prendre 1. Un pas supplémentaire pourrait être de réaliser que cela peut être résumer en: si mon adversaire prend n allumettes, je dois en prendre 4-n. 

Ensuite, on peut se poser la question de la correction de cette stratégie, c'est-à-dire : cette méthode garantit-elle la victoire dans tous les cas ? Il faut donc que, peu importe les coups joués par l'adversaire, j'arrive à une situation gagnante (où je prend la dernière allumette). Pour prouver un tel résultat, on peut d'abord prouver que celle-ci est gagnante avec 4 allumettes (avec ce que l'on appelle une disjonction de cas : pour chaque cas possible -- que mon adversaire prenne 1,2 ou 3 allumettes -- je prend la dernière). Ensuite, en supposant que notre stratégie fonctionne avec un multiple de 4 d'allumettes quelconque (noté par exemple n), alors si l'on rajoute 4 allumettes (et l'on a alors n + 4 allumettes) on peut se ramener au cas avec n allumettes (encore avec une disjontion). Cela montre que si l'on a un multiple de 4 allumettes initialement, alors notre stratégie est gagnante (ce raisonnement est appelé raisonnement par réccurrence -- voir par exemple la page wikipedia \url{https://fr.wikipedia.org/wiki/Raisonnement_par_r%C3%A9currence} pour plus de détails). 








