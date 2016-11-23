##TP1 - Création d'un réseau local : hyperviseur, machine virtuelle, clonage, snapshot, configurations réseaux

###Sudo

L'intérêt d'utiliser `visudo` pour modifier le fichier */etc/sudoers* est que cet outil vérifie la syntaxe du fichier avant d'enregistrer les modifications (et ecraser l'ancienne version). Si on choisi d'utiliser un éditeur de texte simple et qu'on enregistre le fichier avec des erreurs de syntaxe, `sudo` risque de ne plus fonctionner, et puisque */etc/sudoers* n'est modifiable que par *root*, on est coincé (sauf si on a une autre façon d'accéder à *root*.
De plus, il verrouille le fichier pour s'assurer que personne d'autre ne pourrait y accéder pendant la modification. (Pour modifier d'autres fichiers en tant que *root* il existe la commande `sudoedit` qui permet aussi de vérouiller contre les conflits d'édition.)

###Instantané

En essayant de redémarrer la machine virtuelle après l'exécution de `rm -rf /`, la console affiche l'erreur `ne trouve pas le fichier /boot/grub/i386-pc/normal.mod`, et entre dans le mode de récupération grub.
La restauration de l'instantané *Avant rm* permet de retrouver un bon état de fonctionnement.

###Configuration réseaux
Une fois connecté à https://www.duckduckgo.com dans Lynx sur l'invité, le navigateur de l'hôte ne peut pas accéder à https://www.startpage.com/.
