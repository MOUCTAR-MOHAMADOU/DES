# **MANUEL D’UTILISATION DES**

## **Introduction**

Ce rapport présente une implémentation du Data Encryption Standard (DES)
en mode ECB en C. Il compte cinq modules à savoir : main, des,
msg, file et binary ainsi que le makefile. A part le module main, Chacun à un fichier
d’en-tête (.h) et un fichier source (.c). Donc nous allons détaillé la description des modules, la configuration minimale, la compilation et l’exécution du code source.

## **Description des modules**

- main.c est le fichier principal ;
- des.c contient l’algorithme de DES ;
- des.h les prototypes des fonctions de l’algorithme DES ;
- file.c utilitaire permetant de gérer les fichiers à manipuler ‘plaintext.txt et key.txt’ ;
- file.h prototypes des fonctions contenu dans le fichier file.c ;
- msg.c génértion des differnts du trace d’exécution de DES ;
- msg.h prototypes des fonctions contenu dans le fichier msg.c ;
- binaryUtil.c pour la conversion entre binaire et hexadécimal ;
- binaryUtil.h prototypes des fonctions contenu dans le fichier binaryUtil.c ;
- makefile contient les commandes de compilation.

## **Configuration Minimale**

- OS : Linux ;
- GCC : version 11.3 ;
- Utilitaire makefile ;
- text.txt en hexadécimale contenant le texte à chiffré ;
- key.txt en hexadécimale pour la clef à 16 caractères.

## **Compilation**

- Cloner le projet au "https://github.com/MOUCTAR-MOHAMADOU/DES.git"
- Dézipper ‘des.zip’ ;
- Acceder au dossier contenant le code source depuis le terminale ;
- Exécuter la commande ‘make’ pour compiler ;
- Obtention d’un executable ‘des’ après réussite de la compilation.

## **Exécution**

- Créer le fichier et insérer du texte ;
- Le text à chiffré text.txt : "0123456789ABCDEF" ;
- La clef key.txt : "133457799BBCDFF1" ;
- Ouvrir le dossier des depuis un terminal ;
- Exécutable par la commande "make" ;
- Lancer l’exécutable par la commande
"./des" ;
- Suivre les instructions ;
- Obtention des fichier desc.txt et text.txt_cypherText.txt
- desc.txt est un fichier trace ;
- text.txt_cypherText.txt est le chiffré "85e813540f0ab405" ;
- text.txt_cypherText.txt_plainText.txt
est le déchiffrement de text.txt_cypherText.txt qui donne "0123456789abcdef".