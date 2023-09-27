# Zappy

Le Zappy est un projet Epitech consistant au développement d'un jeu en réseau.  
Plusieurs équipes doivent s'affronter sur un terrain contenant des ressources.
L'équipe gagnante est celle avec au moins 6 joueurs qui ont atteint le niveau maximal.  
Ce sont des I.A qui composent les équipes et incarnent les joueurs.

* **Le serveur** a entièrement été développé en C avec les librairies du système Linux.  
* **Les I.A.** ont été développées avec Python 3.  
* **Le client graphique** a été créé en C++ avec la librairie graphique SFML.

## Utilisation

### Lancement du serveur

Après avoir cloné le projet, exécutez la commande ```make``` pour installer le serveur.

Une fois installé, lancez le serveur avec la commande:

```
./zappy_server -p [PORT] -x [WIDTH] -y [HEIGHT] -n [TEAMS] -c [NB_CLIENTS] -f [FREQ]
```

* [PORT]: Port de connexion vers le serveur.

* [WIDTH]: Largeur du terrain.

* [HEIGHT]: Hauteur du terrain.

* [TEAMS]: Noms des différentes équipes qui pourront s'affronter (séparés par des espaces).

* [NB_CLIENTS]: Nombre de joueurs max par équipe.

* [FREQ]: Réciproque du temps pour l'exécution d'actions.

### Lancement de l'I.A

Pour lancer l'I.A., exécutez la commande suivante:

```
./zappy_ai -p [PORT] -n [NAME] -h [MACHINE]
```

* [PORT]: Port de connexion vers le serveur.

* [NAME]: Nom de l'équipe du joueur.

* [MACHINE]: Nom de la machine; localhost par défaut.

### Lancement du client graphique

Pour lancer le client graphique, exécutez la commande suivante:

```
./zappy_gui -p [PORT] -h [MACHINE]
```

* [PORT]: Port de connexion vers le serveur.

* [MACHINE]: Nom de la machine; localhost par défaut.

## Auteurs

* Adèle de Premonville
* Hugo Pattein
* Lucas Holczinger
* Noah Leveve
* Louis Chambon