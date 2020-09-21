# Prise de note Java EE

## Introduction

### Prérequis pour le cours

* des notions en développement Java sont nécessaires;
* des notions en langages HTML et CSS sont préférables, pour une meilleure compréhension des exemples;
* des notions en langage SQL sont préférables, pour une meilleure compréhension de la partie 5 du cours.

### Qu'est-ce que Java EE ?

#### Java EE n'est pas Java ! 

    Le terme "Java" fait référence au langage, mais également à une plate-forme, son nom complet étant "Java SE". 
Celle-ci est constituée de nombreuses bibliothèques, ou API comme `java.lang`, `java.io`, `java.math` ou encore `java.util`.

    Le terme "Java EE" signifie *Java Enterprise Edition*. Il fait quant à lui référence à une extension de la plate-forme standard. 
Autrement dit, la plate-forme Java EE est construite sur le langage Java et la plate-forme Java SE, et elle y ajoute un grand nombre de fonctionnalités que la plate-forme standard n'a pas d'origine. 
L'objectif majeur de Java EE est de faciliter le développement d'applications web robustes et distribuées, déployées et exécutées sur un serveur d'application (comme Tomcat).

#### Java EE n'est pas Javascript

S'il est vrai que Java EE permet la création d'applications web, il ne faut pas pour autant le confondre avec le langage Javascript, souvent raccourci en « JS », qui est lui aussi massivement utilisé dans les applications web. Ce sont là deux langages totalement différents, qui n'ont comme ressemblance que leur nom !

### Internet n'est pas le web !

Avant tout, il ne faut pas confondre l'internet et le web :

    * L'internet et le réseau, le support physique de l'information. Pour faire simple, c'est un ensemble de machines, de câbles et d'éléments réseau en tout genre éparpillés sur la surface du globe;
    * le web constitue une partie seulement du contenu accessible sur l'internet. Vous connaissez et utilisez d'autres contenus, comme le courrier électronique ou encore la messagerie instantanée.

Un site web est un ensemble constitué de pages web (elles-mêmes faites de fichiers HTML, CSS, Javascript, etc.). Lorsqu'on développe puis publie un site web, on met en réalité en ligne du contenu sur internet. On distingue deux types de sites :

    * **les sites internet statiques** : ce sont des sites dont le contenu est « fixe », il n'est modifiable que par le propriétaire du site. Ils sont réalisés à l'aide des technologies HTML, CSS et Javascript uniquement.
    * **les site internet dynamiques** : ce sont des sites dont le contenu est « dynamique », parce que le propriétaire n'est plus le seul à pouvoir le faire changer ! En plus des langages précédemment cités, ils font intervenir d'autres technologies : Java EE est l'une d'entre elles !

### Comment ça marche ?

Lorsqu'un utilisateur consulte un site, ce qui se passe derrière les rideaux est un simple échange entre un client et un serveur.
    * **le client** : dans la plupart des cas, c'est le navigateur installé sur votre ordinateur. Retenez que ce n'est pas le seul moyen d'accéder au web, mais c'est celui qui nous intéresse dans ce cours.
    * **le serveur** : c'est la machine sur laquelle le site est hébergé, où les fichiers sont stockés et les pages web générées.

Le protocole HTTP est utilisé pour donner les normes de communication que tout le monde utilise. Voici les quelques étapes qui constituent un échange simple :
    1. l'utilisateur saisit une URL dans la barre d'adresses de son navigateur;
    2. le navigateur envoie alors une requête HTTP au serveur pour lui demander la page correspondante;
    3. le serveur reçoit cette requête, l'interprète et génère alors une page web qu'il va renvoyer au client par le biais d'une réponse HTTP;
    4. le navigateur reçoit, via cette réponse, la page web finale, qu'il affiche alors à l'utilisateur.

Le navigateur permet d'interpréter les pages web ainsi reçues. Elles ne contiennent alors que du code HTML, CSS et JavaScript. Seul le code source du serveur peut être du Java EE qui permet de créer de manière dynamique les pages web retournées au client.

Pour choisir la technologie la plus adaptée à son projet, plusieurs facteurs rentrent souvent en compte :
    * l'expérience personnelle : si vous avez déjà développé en Java, Python ou C# auparavant, il semble prudent de vous orienter respectivement vers Java EE, Django et .NET;
    * vos besoins : rapidité de développement, faible utilisation des ressources sur le serveur, réactivité de la communauté soutenant la technologie, ampleur de la documentation disponible en ligne, coût, etc.
