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
* Python (pour le monitoring, le stop and start des serveurs et le rcon)
    - Flask (pour la gestion du server web)

## Avancement :

Séances :
- 09/11/2022 :
   * Durant cette séance :
   Poursuite du projet serveur minecraft Bungee Cord (avec des nouveaux bonus)
   * Pour la prochaine séance :
   Avancée sur le projet.

- 23/11/2022 :
   * Durant cette séance :
   Avancée sur le projet serveur minecraft Bungee Cord découverte de Docker
   * Pour la prochaine séance :
   Mise en place du PC (16go RAM, i7) (que j'ai reçu)
   Avancée sur la decouverte de Docker

- 07/12/2022 :
   * Durant cette séance :  
   Avancée sur le projet serveur minecraft :
      - Changement de bungee cord pour velocity
      - Mise en place de velocity
      - Mise en place d'un serveur fabric (qui ne marche pas encore)
   * Pour la prochaine séance :
      - Avancée sur le serveur fabric

- 04/01/2023 :
   * Durant cette séance :
   Avancée sur le projet serveur minecraft :
      - Résolution du problème du /lobby ou /hub
      - Installtion de luckperms velocity
      - Mise en place du stop and start des serveurs
      - Intervention d'un dirlab du labo Cyber

- 18/01/2023 :
   * Entre la séance :
      - Résolution du problème du /lobby ou /hub
      - Correction des fix du stop and start des serveurs
      - Changement des modèles de serveurs (du paper --> Miraï)
      - Changement de Java (openjdk --> GraalVM)
      - Ajout de l'authentification sur les serveurs de Mojang/Microsoft (donc réparation des skins)
   * Durant cette séance :
      - Ajout d'un plugin de maintenance (qui peux mettre velocity en maintenance ou chaque serveur individuellement)
      - Configuration du RCON (pour pouvoir stop and start les serveurs proprement)

## Problèmes rencontrés :

* Stop and start des serveurs :
    - Au début mes serveurs fonctionnaient dans des screens (ce qui ne facilite pas le stop and start des serveurs)
    - J'ai donc changé tout en systemd (ce qui a été plus simple pour le stop and start des serveurs)

