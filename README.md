## Tablut – Jeu & Intelligence Artificielle (Java)
Ce projet implémente le jeu Tablut avec :
 -une IA jouable (algorithmes de recherche / heuristiques)
 - un mode réseau via un serveur central
 - une architecture modulaire (moteur de jeu, IA, réseau)
 - un système de build via make

## Fonctionnalités principales
IA utilisant des stratégies de recherche (minimax/heuristiques)
Mode multijoueur réseau avec serveur central
Exécution console
Build automatisé via Makefile

## Compilation & exécution
 
 # Compilation + exécution
 
 make run

 # Commandes annexes

- Compiler uniquement :
make
- Nettoyer les .class :
make clean
- Recompiler proprement :
make rebuild

 # Mode réseau
1. Compiler :
make
2️. Lancer le serveur central :
java -cp bin tablut.network.ServeurCentral

3️.Démarrer les joueurs :
un joueur en host
un autre en join
Le serveur assure la communication entre les deux joueurs.

# Générer un fichier JAR
Créer un fichier MANIFEST.MF :
Main-Class: tablut.Main

(⚠️ Ligne vide obligatoire)
. Commande pour générer le JAR :
jar cfm MonApp.jar MANIFEST.MF -C bin . -C res . -C temp .
