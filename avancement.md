{\rtf1\ansi\ansicpg1252\cocoartf1561\cocoasubrtf610
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 Veuillez renseigner votre avancement \'e0 chaque \'e9tape achev\'e9e et test\'e9e et par d\'e9faut \'e0 la fin de chaque s\'e9ance de TP \
##############\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 # Partie 1 du BE \
##############\
\
\
## Version 1 de tsock \
########## \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 L'objectif principal de la 1\'e8re s\'e9ance est de d\'e9velopper la v1 de tsock: coder une version de la source et une version du puit capables d'\'e9changer des messages en utilisant le service UDP. \
Vous pouvez d\'e9composer le travail en deux parties successives : la version "source" de "tsock" puis celle du "puit". Vous pouvez tester chaque \'e9tape de mani\'e8re isol\'e9e, en utilisant la version enseignant de tsock (en la configurant comme puit, pour tester votre source ou en tant que sourcenetcat , pour votre version du puit).  Cela n\'e9anmoins suppose que vous soyez connect\'e9(e) sur une machine INSA via le client VPN. A d\'e9faut, vous pouvez  utiliser l'utilitaire nc (netcat), disponible sous les diff\'e9rents syst\'e8mes d'exploitation. \
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 ### Point sur la partie SOURCE UDP\
###############\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 veuillez cocher les seules cases qui correspondent aux \'e9tapes valid\'e9es.  \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
[ ] la gestion des options -s, -u,  le nombre et Taille par d\'e9faut des messages , nom de la machine destinataire,  num\'e9ro de port du puit est op\'e9rationnelle\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la cr\'e9ation du socket UDP local et la construction de l'adresse du socket distant est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
[ ] l\'92envoi de  messages en utilisant l'appel syst\'e8me sendto (qui retourne une valeur >0 correspondant \'e0 la taille de chaque message envoy\'e9) est fonctionnelle \
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la r\'e9ception c\'f4t\'e9 puit (sur nc ou la version "enseignant" de tsock) des messages envoy\'e9s par votre client est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
### Point sur la partie puit UDP.\
#############\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la prise en compte de l' option -p est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la cr\'e9ation du socket UDP local du puit et la construction de son adresse est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
[ ] la r\'e9ception et l'affichage des messages re\'e7us sont corrects\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] l'\'e9change de messages tq d\'e9crits dans le cahier des charges entre vos versions source et puit de la version 1 de "tsock" est op\'e9rationnel\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
################\
## avancement sur la version 2 de tsock\
###############\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 La version 2 int\'e8gre l\'92utilisation de TCP pour l\'92\'e9change des messages. Veuillez renseigner les \'e9tapes que vous avez trait\'e9es.  \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
[ ] la cr\'e9ation du socket TCP local du puit et la construction de son adresse est correcte\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] l'acceptation de la demande d'\'e9tablissement de connexion de la primitive "accept" est effective \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la r\'e9ception et l'affichage des messages re\'e7us  (en utilisant nc ou la version "enseignant" de tsock comme source)  sont corrects \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] l'\'e9change de messages entre vos versions source et puit de la version 1 de "tsock" est op\'e9rationnel\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
##################\
## avancement version 3 de tsock\
##################\
\
La version v3 de tsock int\'e8gre les fonctions de formatage et d'affichage des messages \'e9mis et re\'e7us (selon le cahier des charges) ainsi que la gestion des options restantes : -n  et -l\
Si toutes les fonctionnalit\'e9s additionnelles de la version 3 sont valid\'e9es par vos tests, vous devez cocher toutes les cases suivantes. Si ce n'est pas le cas, veuillez cocher les seules cases qui correspondent aux \'e9tapes valid\'e9es.  \
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] Le formattage et affichage des messages selon le cahier des charges sont op\'e9rationnels\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la prise en compte de l'option -n en \'e9mission aussi bien avec UDP et TCP est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la prise en compte de l'option -n en r\'e9ception avec UDP est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la prise en compte de l'option -n en r\'e9ception avec TCP est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] la prise en compte de l'option -l est correcte\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
##################################################\
# Avancement PARTIE 2 du BE : Syst\'e8me de boites aux lettres \
##################################################\
\
\
Tr\'e8s grossi\'e8rement, comme indiqu\'e9 dans la simplification du sujet de BE qui vous a \'e9t\'e9 transmise vous aurez successivement \'e0 d\'e9velopper : \
	- l\'92Emetteur  (l'option "-e" de tsock) : qui est une adaptation de la version v3 du "tsock" (de la premi\'e8re partie) pour principalement  demander l'\'e9tablissement de connexion TCP avec le serveur BAL \
	- Transmettre le PDU applicatif en charge de le d\'e9clarer en tant que \'e9metteur et \'e9ventuellement indiquer la taille et nombre de messages qu'il \'e9met\
	- Emettre les messages au serveur BAL clore la connexion TCP\
\
Les fonctionnalit\'e9s du serveur BAL (option "-b") relatives aux interactions avec les Emetteurs pour :\
	- accepter les demandes de connexions TCP et l'identification,par le traitement du PDU applicatif, du r\'f4le "Emetteur" de l'application qui a initi\'e9e la demande de connexion et ses caract\'e9ristiques  (nombre et taille des messages) \
	- prendre en charge les fonctions en lien avec la manipulation de la structure de donn\'e9es propos\'e9es (i.e. liste cha\'een\'e9e de boites aux lettres (BAL), d'une liste cha\'een\'e9e des messages d'une BAL) en r\'e9action aux envois de messages d'une application "Emetteur"\
	- recherche de BAL relative \'e0 un r\'e9cepteur\
	- creation/rajout de BAL d'un r\'e9cepteur\
	- rajout d'un message dans une BAL d'un r\'e9cepteur \'e0 la derni\'e8re position\
\
Les fonctionnalit\'e9s du serveur BAL (option "-b") relatives aux interactions avec les r\'e9cepteurs pour :\
	- accepter les demandes de connexions TCP et l'identification, par le traitement du PDU applicatif, du r\'f4le "R\'e9cepteur" de l'application qui a initi\'e9e la demande de connexion\
	- prendre en charge les fonctions en lien avec la manipulation de la structure de donn\'e9es pour le compte d'une application "R\'e9cepteur" :\
	- v\'e9rifier la pr\'e9sence d'une BAL associ\'e9e \'e0 un r\'e9cepteur et renvoyer l'acc\'e8s \'e0 la liste des messages disponibles pour le r\'e9cepteur  \
- parcours des messages d'une BAL\
\
Le R\'e9cepteur  (l'option "-r" de tsock) : qui est une adaptation de la version v3 du "tsock" (de la premi\'e8re partie) pour principalement : \
	- demander l'\'e9tablissement de connexion TCP avec le serveur BAL\
	- Transmettre le PDU applicatif en charge de le d\'e9clarer en tant que r\'e9cepteur 	- prendre en charge la r\'e9ception et affichage de ses \'e9ventuels messages transmis par le serveur BAL jusqu'\'e0 la fermeture de la connexion TCP d\'e9clench\'e9e par le serveur BAL\
\
\
## Pour ce qui est de l'\'e9metteur (l'option "-e" de tsock)\
#############################\
 veuillez indiquer les \'e9tapes que vous avez valid\'e9es.\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] demande d'\'e9tablissement de connexion TCP avec le serveur BAL fonctionnelle\
\pard\pardeftab720\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] transmission du PDU applicatif en charge de le d\'e9clarer en tant que \'e9metteur et \'e9ventuellement indiquer la taille et nombre de messages qu'il \'e9met est fonctionnelle\
\pard\pardeftab720\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] \'e9mission des messages au serveur BAL fonctionnelle\
\pard\pardeftab720\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] cloture de la connexion TCP avec le serveur BAL fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
## Pour les fonctionnalit\'e9s du serveur BAL (option "-b") relatives aux interactions avec les Emetteur\
#############################\
veuillez indiquer \'e9tapes que vous avez valid\'e9es\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] Acceptation des demandes de connexions TCP et l'identification,par le traitement du PDU applicatif, du r\'f4le "Emetteur" de l'application qui a initi\'e9e la demande de connexion et ses caract\'e9ristiques  (nombre et taille des messages)  est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] recherche de la bo\'eete aux lettres (BAL) relative \'e0 un r\'e9cepteur fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] creation/rajout de BAL d'un r\'e9cepteur fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] rajout d'un message dans une BAL d'un r\'e9cepteur \'e0 la derni\'e8re position est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
## Pour les fonctionnalit\'e9s du serveur BAL (option "-b") relatives aux interactions avec les R\'e9cepteurs\
#####################\
 veuillez indiquer les \'e9tapes que vous avez valid\'e9es\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] acceptation des demandes de connexions TCP et l'identification, par le traitement du PDU applicatif, du r\'f4le "R\'e9cepteur" de l'application qui a initi\'e9e la demande de connexion est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] v\'e9rification de la pr\'e9sence d'une BAL associ\'e9e \'e0 un r\'e9cepteur et renvoi de l'acc\'e8s \'e0 la liste des messages disponibles pour le r\'e9cepteur est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\
\
## Pour ce qui est du "R\'e9cepteur" (l'option "-e" de tsock) \
################\
veuillez indiquer les \'e9tapes que vous avez valid\'e9es.\
\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] demande de l'\'e9tablissement de connexion TCP avec le serveur BAL est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] Transmission du PDU applicatif en charge de le d\'e9clarer en tant que r\'e9cepteur  est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] prise en charge la r\'e9ception et affichage de ses \'e9ventuels messages transmis par le serveur BAL jusqu'\'e0 la fermeture de la connexion TCP d\'e9clench\'e9e par le serveur BAL est fonctionnelle\
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 \
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0
\cf0 [ ] parcours des messages d'une BAL op\'e9rationnel}