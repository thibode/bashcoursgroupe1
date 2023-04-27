## Exercice pratique : Gestion de fichiers en shell

Dans cet exercice, nous allons utiliser les commandes de base du shell pour manipuler des fichiers et des répertoires.

### Énoncé

1.  Créez un répertoire nommé "documents" à la racine de votre système de fichiers.
2.  Créez un fichier vide nommé "note.txt" dans le répertoire "documents".
3.  Ajoutez le texte suivant au fichier "note.txt" :
    `Ceci est ma première note.`
4.  Dupliquez le fichier "note.txt" et nommez la copie "note_backup.txt".
5.  Affichez le contenu des fichiers "note.txt" et "note_backup.txt" à l'aide d'une seule commande.
6.  Renommez le fichier "note_backup.txt" en "backup_note.txt".
7.  Créez un répertoire nommé "images" dans le répertoire "documents".
8.  Copiez un fichier image de votre choix dans le répertoire "images".
9.  Affichez la taille du fichier image en kilooctets.
10. Affichez la liste de tous les fichiers et répertoires présents dans le répertoire "documents", y compris les fichiers cachés.

11. Supprimez le répertoire "images" et tous ses fichiers et sous-répertoires.

12. Supprimez le fichier "note.txt".

### Correction

1.  Pour créer un répertoire nommé "documents" à la racine de votre système de fichiers, utilisez la commande suivante :
    `sudo mkdir /documents`

    Remarque : vous devez utiliser "sudo" pour exécuter cette commande en tant qu'administrateur.

2.  Pour créer un fichier vide nommé "note.txt" dans le répertoire "documents", utilisez la commande suivante :
    `touch /documents/note.txt`
3.  Pour ajouter le texte "Ceci est ma première note." au fichier "note.txt", utilisez la commande suivante :
    `echo "Ceci est ma première note." > /documents/note.txt`
4.  Pour dupliquer le fichier "note.txt" et nommer la copie "note_backup.txt", utilisez la commande suivante :
    `cp /documents/note.txt /documents/note_backup.txt`
5.  Pour afficher le contenu des fichiers "note.txt" et "note_backup.txt" à l'aide d'une seule commande, utilisez la commande suivante :
    `cat /documents/note.txt /documents/note_backup.txt`
6.  Pour renommer le fichier "note_backup.txt" en "backup_note.txt", utilisez la commande suivante :
    `mv /documents/note_backup.txt /documents/backup_note.txt`
7.  Pour créer un répertoire nommé "images" dans le répertoire "documents", utilisez la commande suivante :
    `mkdir /documents/images`
8.  Pour copier un fichier image de votre choix dans le répertoire "images", utilisez la commande suivante :
    `cp chemin_vers_l_image /documents/images`

9.  Pour afficher la taille du fichier image en kilooctets, utilisez la commande suivante :
    `du -sh /documents/images/nom_du_fichier`

    Remarque : vous devez remplacer "nom_du_fichier" par le nom du fichier image que vous avez copié.

10. Pour afficher la liste de tous les fichiers et répertoires présents dans le répertoire "documents", y compris les fichiers cachés, utilisez la commande suivante :
    `ls -la /documents`

11. Pour supprimer le répertoire "images" et tous ses fichiers et sous-répertoires, utilisez la commande suivante :
    `rm -rf /documents/images`

12. Pour supprimer le fichier "note.txt", utilisez la commande suivante :
    `rm /documents/note.txt`
