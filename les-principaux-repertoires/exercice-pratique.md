1.  Créez un nouveau répertoire appelé "exercice_shell" dans votre répertoire personnel en utilisant la commande suivante :
    `mkdir ~/exercice_shell`
2.  Déplacez-vous dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `cd ~/exercice_shell`
3.  Créez un nouveau répertoire appelé "niveau1" dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `mkdir niveau1`
4.  Déplacez-vous dans le répertoire "niveau1" en utilisant la commande suivante :
    `cd niveau1`
5.  Créez un nouveau fichier appelé "fichier_niveau1.txt" dans le répertoire "niveau1" en utilisant la commande suivante :
    `touch fichier_niveau1.txt`
6.  Affichez le chemin absolu du répertoire "niveau1" en utilisant la commande suivante :
    `pwd`

    Notez le chemin absolu affiché.

7.  Déplacez-vous dans le répertoire parent en utilisant la commande suivante :
    `cd ..`
8.  Créez un nouveau répertoire appelé "niveau2" dans le répertoire "exercice_shell" en utilisant la commande suivante :
    `mkdir niveau2`
9.  Déplacez-vous dans le répertoire "niveau2" en utilisant la commande suivante :
    `cd niveau2`
10. Créez un nouveau fichier appelé "fichier_niveau2.txt" dans le répertoire "niveau2" en utilisant la commande suivante :
    `touch fichier_niveau2.txt`

11. Créez un nouveau lien symbolique appelé "lien_niveau1" dans le répertoire "niveau2" qui pointe vers le répertoire "niveau1" en utilisant la commande suivante :
    `ln -s ~/exercice_shell/niveau1 lien_niveau1`

12. Affichez le chemin absolu du lien symbolique "lien_niveau1" en utilisant la commande suivante :
    `readlink -f lien_niveau1`


    Notez le chemin absolu affiché.

13. Supprimez le fichier "fichier_niveau2.txt" en utilisant la commande suivante :
    `rm fichier_niveau2.txt`

14. Supprimez le répertoire "niveau2" et tous ses fichiers et sous-répertoires en utilisant la commande suivante :
    `rm -rf ~/exercice_shell/niveau2`
