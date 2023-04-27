## Énoncé

Vous êtes en charge de la gestion des backups d'une entreprise. Vous avez pour mission de créer un script shell qui effectue une copie de sauvegarde des fichiers importants de l'entreprise et les stocke dans un dossier dédié.

Les fichiers importants sont situés dans les dossiers suivants :

- `/var/www/html`
- `/etc/apache2`
- `/home/user/Documents`

Le script doit effectuer les actions suivantes :

1.  Vérifier que l'utilisateur a les permissions nécessaires pour exécuter le script.
2.  Créer un nouveau dossier de sauvegarde appelé `backup`.
3.  Copier les fichiers importants dans le dossier `backup`.
4.  Archiver le dossier `backup` dans un fichier `tar.gz` appelé `backup.tar.gz`.
5.  Supprimer le dossier `backup`.

## Correction

Voici la correction du script shell pour effectuer la sauvegarde des fichiers importants :
Vérifier que l'utilisateur a les permissions nécessaires pour exécuter le script

    if [ $(id -u) -ne 0 ]; then
      echo "Vous devez être root pour exécuter ce script."
      exit 1
    fi

Créer un nouveau dossier de sauvegarde appelé "backup"

    mkdir backup

Copier les fichiers importants dans le dossier "backup"

    cp -r /var/www/html backup/
    cp -r /etc/apache2 backup/
    cp -r /home/user/Documents backup/

Archiver le dossier "backup" dans un fichier tar.gz appelé "backup.tar.gz"

    tar -czvf backup.tar.gz backup

Supprimer le dossier "backup"

    rm -r backup
