# Compte rendu projet serveur minecraft Velocity

Lien répertoire github : https://github.com/Wiibleyde/bungee-server (Entre temps le nom n'est plus à jour car bungee cord a été changé par velocity)
## Projet :

Le projet est de mettre en place un serveur minecraft avec un proxy qui est en capacité de rediriger les joueurs vers les serveurs.

Pour ma part j'ai 4 serveurs : 
* Serveur lobby
* Serveur survival
* Serveur creative
* Serveur privé (pour les amis)

Tous ces serveurs fonctionnent avec Mirai (fork de Paper) et sont en version 1.19.2.

Le proxy que j'ai choisi est Velocity, car il est plus puissant que BungeeCord, plus foncionnel et plus optimisé.

De plus j'ai rajouté une page de monitoring pour voir les joueurs connectés sur chaque serveur.
Lien de la page de monitoring : [https://minecraft.bonnell.fr/](https://minecraft.bonnell.fr/)

J'ai rajouté plusieurs plugins pour gérer les permissions, les skins, les serveurs, les messages, etc...

Plugins :
* Velocity :
    - LuckPerms Velocity
    - Maintenance Velocity
    - SkinRestorer Velocity
    - Slashhub Velocity

* Serveurs :
    - LuckPerms
    - WorldEdit (FAWE)
    - Holographic Displays (Lobby seulement)
    - EssentialsX
    - EssentialsXSpawn
    - EssentialsXChat

Pour faire fonctionner mes serveurs, au départ j'avais un PC portable vieux de 15 ans avec 4GO de RAM et un vieux i3, mais au final la config de mon serveur minecraft est :
* 16GO de RAM
* i7 
* 512GO de SSD SATA M.2

Les technologies que j'ai utilisé sont :
* Systemd (pour le lancement des serveurs et du proxy)
* GraalVM (Java mais avec une meilleure optimisation)
* Python (pour le monitoring et le stop and start des serveurs)
    - Flask (pour la gestion du server web)

## Problèmes rencontrés :

* Stop and start des serveurs :
    - Au début mes serveurs fonctionnaient dans des screens (ce qui ne facilite pas le stop and start des serveurs)
    - J'ai donc changé tout en systemd (ce qui a été plus simple pour le stop and start des serveurs)

