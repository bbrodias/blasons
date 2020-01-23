# Lien entre l'activité des blasons et l'informatique

On utilise ici à la fois la classification en 4 concepts (Algorithme,
Langage, Information et données, et Machine) que l'on retrouve à
plusieurs niveaux dans les programmes français, et la classification
en (six compétences de la pensée informatique)[https://csunplugged.org/en/computational-thinking/]
dues à Tim Bell et ses collègues de CS unplug.

On s'attache également à se raccrocher à des éléments de la vie de
tous les jours pour raccrocher ces concepts au vécu des participants.

## Concepts de l'informatique

### Langage (\*\*: très adaptée)

Cette activité a été inventée pour mettre en valeur le concept de
Langage en informatique. L'objectif est de parvenir à communiquer
efficacement la description exacte de différents motifs (qui sont ici
des blasons) : la description doit être suffisamment précise pour que
celui qui la reçoive puisse redessiner le plus fidèlement possible le
blason original. 

Au cours de l'activité, les participants comprennent la nécessité de
définir et utiliser un langage spécifique et adapté à la tâche. Il est
nécessaire de définir les mots et expressions autorisés (ce que l'on
appelle la *syntaxe*), ainsi que leur signification (ce que l'on
appelle la *sémantique*).
 	
Cette activité permet également d'explorer différentes
caractéristiques décrivant les différents langages.  Tout d'abord,
*l'expressivité* d'un langage détermine l'ensemble des objets que le
langage peut décrire. Dans l'activité, la fiche B propose des motifs
faciles à décrire dans le langage induit par la fiche de vocabulaire,
mais la fiche C propose des motifs montrant les limites de ce langage.
On peut ainsi mesurer l'expressivité du langage de blasonnement au
nombre de motifs qu'il peut décrire.

De manière générale, un langage ne peut pas tout décrire. Par exemple,
un langage permettant de décrire des segments de droite ne permettra
pas de décrire un cercle. On peut décider d'étendre un langage pour le
rendre plus expressif, en le complexifiant. Il reste formellement
impossible de faire un langage se décrivant entièrement lui-même.
 	
D'autre part, la définition d'un langage pose la question de son
*ambiguïté*. C'est une question liée à la sémantique (aux
significations associées au signes): Le langage est dit ambiguë si
plusieurs significations peuvent être associées à une même
description. Par exemple, dire "coupe la figure en deux parties" est
ambiguë si on ne précise pas s'il faut le faire verticalement ou
horizontalement, ou si on ne précise pas si les parties doivent être
de même taille ou non.

Une langue laissant de la place aux ambiguités (comme le Français) est
plus adaptée pour décrire des sentiments ou faire de la poésie, mais
elle ne convient pas pour communiquer avec l'ordinateur. C'est l'une
des raisons pour lesquelles la notion de Langage est primordiale en
informatique.

Plus précisément, lorsque l'on veut décrire un algorithme à un
ordinateur pour que celui-ci puisse l'exécuter, on a besoin d'un
langage qui puisse être compris par cet ordinateur. C'est ce que l'on
appelle un langage de programmation (ces langages permettent donc
d'écrire des programmes). A noter que l'on perçoit ici clairement la
différence entre un algorithme, qui dans le cas de la description de
blasons, cela correspondrait à leur description en français, et un
programme, qui correspondrait à leur description plus formelle dans le
langage que l'on s'est donné. Les notions abordées précédemment,
d'expressivité et de non ambiguïté, sont essentielles dans
l'élaboration d'un langage de programmation, pour que n'importe quel
algorithme puisse être décrit dans ces langages, ainsi que pour que
les programmes écrits dans ces langages ne puissent être interprétés
que d'une unique manière. Ce dernier point est particulièrement
important si l'on veut pouvoir certifier que l'exécution d'un
programme se déroule de la manière attendue. Il serait en effet peu
souhaitable que les programmes responsables du déploiement des
airbags dans une voiture ne suivent pas le comportement attendu.

### Information et Données (\*: Adaptée)

Cette activité peut être utilisée pour discuter de représentation d'un
image dans la mémoire d'un ordinateur (en lien avec le concept de
Données). C’est plus facile si la classe a joué l’activité de CS
unplug sur représentation bitmap des images, mais cela reste possible
sinon.

Les représentations bitmap (gif ou png) et vectorielle (pdf) des
images sont très complémentaires. Une fois que l’idée générale d'image
bitmap est comprise, l’animateur peut expliquer comment les bitmaps
sont mal adaptés au zoom aggrandissant alors que les images
vectorielles garde la même qualité à toutes les échelles (l’impression
d’une image pixelisée aide cette discussion).

Le format pdf, initialement prévu pour imprimer les documents, est
avant tout vectoriel même si on peut également inclure des bitmaps
dans un pdf. La façon de décrire les pages web en HTML est assez
proche d'une représentation vectorielle (on décrit quels éléments
doivent apparaitre où à l'écran), tout comme les sauvegardes d'un
traitement de texte.

On peut aussi discuter de la taille de telles images pour parler de
l'efficacité de ces représentations. Les images vectorielles sont
clairement mieux adaptées pour les blasons: taille mémoire plus faible
et meilleure qualité de zoom. À l'inverse, stocker l'image d'un
paysage est probablement difficile en utilisant une image vectorielle
(on pourrait argumenter que les ondelettes des fichiers jpg sont une
amélioration des images vectorielles, mais c'est largement hors sujet.
L'animateur doit juste rester prudent en n'affirmant pas qu'il est
impossible de représenter une image réaliste sous forme de vecteur).


De manière optionnelle, on peut également aborder des idées plus
abstraites autour du concept d'information. On peut se demander pour
cela comment ont été triés les blasons entre les feuilles A et B. Tous
peuvent être décrits avec le langage proposé, mais certains sont
clairement plus complexes que d’autres. Comment quantifier cela?
Comment trier les blasons par complexité croissante, par exemple?

Ce que nous avons fait pour construire cette activité a été d’écrire
la représentation de chaque blason, puis de les trier en fonction de
la longueur de la description: plus longue est la description, plus le
blason doit être complexe. C'est cependant contestable, car certains
des blasons de la feuille C auraient pu être placé sur la feuille B
avec un langage légèrement différent.

Cela conduit à un question très profonde: quelle est la quantité
minimale de signes à utiliser pour représenter sans ambiguïté un
blason donné? Une réponse précise va bien au-delà de cette activité,
mais vous pouvez obtenir une première approximation sur votre
ordinateur: il suffit de compresser ce fichier dans un .zip, et de
mesurer la taille du fichier resultant.

### Algorithme (.)

Il y a assez peu de lien avec cette activité. On peut discuter de la
différence entre algorithme et programme en terme de formalisme. Voir
la section Langage pour plus de détails.
 
### Machine (.)

Il n'y a pas de lien avec cette activité.
 
## Compétences de la pensée informatique

### Abstraction/Modélisation (\*)
Lors de la description d'un blason, celui-ci doit être vu (c'est-à-dire modélisé) comme une suite d'instructions pour qu'il puisse être décrit efficacement. Ainsi, la suite d'instructions correspondant au blason s'abstrait de la forme précise de celui-ci. 

### Décomposition (\*)
Lors de la description d'un blason, celui-ci doit être décomposé en parties plus petites de telles manières que chacunes de ces parties puissent être facilement décrites. Typiquement, on découpe d'abord différentes parties du blason avant de décrire comment celles-ci sont remplies. La description d'un blason passe donc par la décomposition de celui-ci en parties plus petites et plus simples de telle manière que celles-ci puissent être décrites sans avoir besoin de les décomposer plus avant.

### Généralisation et motifs (\*\*)
Si les participants élaborent eux-même un langage de description de blasons, cela est fait à partir de leur expérience de la description de quelques blasons. Il faut alors repérer les motifs (qu'il soient géométriques ou au sein des descriptions de blasons) qui apparaissent pour pouvoir élaborer un langage. De plus, lorsqu'ils se rendent compte que le langage mis en place n'est plus suffisant pour décrire un blason en particulier, il faut pouvoir mettre en lumière la ou les partie(s) du blason qui ne peuvent être décrites. A partir de celle(s)-ci, si les participants veulent mettre à jour le langage pour qu'ils puissent décrire plusieurs nouveaux blasons, il faut trouver un ensemble de motifs qui ne peuvent pas être décrit par le langage. Ainsi, un problème observé sur un exemple doit pouvoir permettre de généraliser à un problème sur le langage lui-même.
	
### Évaluation (\*)
Au cours de l'activité, les participants doivent, à partir de la description d'un blason, essayer de le reproduire. Une fois que cela est fait, il faut évaluer le résultat, c'est-à-dire estimer à quel point ce qui est dessiné est proche de ce qui a été décrit. Plusieurs méthodes d'évaluation peuvent être utilisées. Par exemple, on peut utiliser une simple évaluation binaire du type : "le dessin est identique" et "le dessin est différent". On peut également être plus nuancé en définissant la différence entre un dessin et le blason original par le nombre d'instructions nécessaires pour corriger le dessin. Enfin, on peut aussi regarder quelle est l'instruction qui n'a pas été comprise de la façon voulue.

Lorsque l'on se rend compte que l'on n'arrive pas à décrire adéquatement un blason avec le langage que l'on s'est donné, si l'évaluation est simplement binaire, on ne peut pas se rendre compte de l'origine du problème (l'expressivité ou l'ambiguïté du langage utilisé, voir la section Langage). Une évaluation plus précise des différences entre un dessin et l'original permet alors une évaluation du langage de description lui-même, qui peut ensuite être modifié pour être plus adapté aux blasons suivants.

### Pensée algorithmique (.)
Cette activité n'est pas centrée sur la notion d'algorithme, mais elle illustre tout de même le séquençage d'instructions nécessaire pour la description des blasons. Notamment, via la description des blasons passent par leur décomposition (que l'on peut vouloir)

Typiquement, on découpe d'abord différentes parties du blason avant de décrire comment celles-ci sont remplies. Ainsi, la description d'un blason s'apparente à une suite d'instructions, et nécessite donc d'utiliser une pensée algorithmique. Il faut tout de même remarquer qu'un algorithme décrivant un blason donné est un peu particulier étant donné qu'il renvoie toujours la même chose. 
	
### Logique (.)

