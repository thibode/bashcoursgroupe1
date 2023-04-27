1.  Créez un nouveau répertoire appelé "exercice_shell" dans votre répertoire personnel en utilisant la commande suivante :
    `mkdir ~/exercice_shell`
2.  Déplacez-vous dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `cd ~/exercice_shell`
3.  Créez un nouveau fichier appelé "fichier_test.txt" dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `touch fichier_test.txt`
4.  Affichez le contenu du fichier "fichier_test.txt" en utilisant la commande suivante :
    `cat fichier_test.txt`

    Notez que le fichier est vide.

5.  Ajoutez le texte "Bonjour le monde!" au fichier "fichier_test.txt" en utilisant la commande suivante :
    `echo "Bonjour le monde!" >> fichier_test.txt`
6.  Affichez à nouveau le contenu du fichier "fichier_test.txt" en utilisant la commande suivante :
    `cat fichier_test.txt`

    Notez que le texte "Bonjour le monde!" a été ajouté au fichier.

7.  Renommez le fichier "fichier_test.txt" en "fichier_modifie.txt" en utilisant la commande suivante :
    `mv fichier_test.txt fichier_modifie.txt`
8.  Affichez la liste des fichiers et des répertoires dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `ls`

    Notez que le fichier "fichier_modifie.txt" est maintenant présent dans le répertoire.

9.  Copiez le fichier "fichier_modifie.txt" dans un nouveau fichier appelé "fichier_copie.txt" en utilisant la commande suivante :
    `cp fichier_modifie.txt fichier_copie.txt`
10. Affichez la liste des fichiers et des répertoires dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `ls`


    Notez que le fichier "fichier_copie.txt" est maintenant présent dans le répertoire.

11. Supprimez le fichier "fichier_modifie.txt" en utilisant la commande suivante :
    `rm fichier_modifie.txt`

12. Créez un nouveau répertoire appelé "nouveau_repertoire" dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `mkdir nouveau_repertoire`

13. Déplacez le fichier "fichier_copie.txt" dans le répertoire "nouveau_repertoire" en utilisant la commande suivante :
    `mv fichier_copie.txt nouveau_repertoire/`

14. Affichez la liste des fichiers et des répertoires dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `ls`


    Notez que le fichier "fichier_copie.txt" a été déplacé dans le répertoire "nouveau_repertoire".

15. Supprimez le répertoire "nouveau_repertoire" et tous ses fichiers et sous-répertoires en utilisant la commande suivante :
    `rm -rf`
