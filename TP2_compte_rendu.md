##TP2 - Création d'un réseau local : la passerelle

###Feuille de route

0\. Cartes réseaux déjà configurées (?).  
1. Sur la passerelle: `sudo apt-get install openssh-server` puis `sudo service ssh start` pour démarrer le serveur.  
2. Pour se connecter à partir de l'hôte en tant qu'utilisateur courant: `ssh pb@192.168.99.47`. Quand on essaie de se connecter en tant que `root`, un message indique qu'on n'a pas la permission.  
3. `sudo nano /etc/ssh/sshd_config` pour accéder au fichier de configuration; modification du port 22 au port 26. (cf. http://www.faqs.org/docs/securing/chap15sec122.html)  
4.   
