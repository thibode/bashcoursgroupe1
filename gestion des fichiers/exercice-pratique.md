## Exercice pratique : Manipulation de fichiers avec le shell

Dans cet exercice, nous allons utiliser les commandes de base du shell pour manipuler des fichiers.

### Énoncé

1.  Créez un répertoire nommé "mon_projet".
2.  Créez un fichier vide nommé "README.md" dans le répertoire "mon_projet".
3.  Affichez le contenu du répertoire "mon_projet".
4.  Créez un fichier nommé "index.html" dans le répertoire "mon_projet". Le fichier doit contenir le texte suivant :

    <!DOCTYPE html>

        <html>
          <head>
            <title>Mon projet</title>
          </head>
          <body>
            <h1>Bienvenue sur mon projet !</h1>
          </body>
        </html>`

5.  Affichez le contenu du fichier "index.html".
6.  Dupliquez le fichier "index.html" et nommez la copie "index_backup.html".
7.  Affichez le contenu du répertoire "mon_projet" pour vérifier que les deux fichiers "index.html" et "index_backup.html" existent.
8.  Renommez le fichier "index_backup.html" en "backup.html".
9.  Affichez le contenu du répertoire "mon_projet" pour vérifier que le fichier "backup.html" a été correctement renommé.

### Correction

1.  Pour créer un répertoire nommé "mon_projet", utilisez la commande suivante :

    `mkdir mon_projet`

2.  Pour créer un fichier vide nommé "README.md" dans le répertoire "mon_projet", utilisez la commande suivante :

    `touch mon_projet/README.md`

3.  Pour afficher le contenu du répertoire "mon_projet", utilisez la commande suivante :

    `ls mon_projet`

4.  Pour créer un fichier nommé "index.html" dans le répertoire "mon_projet", utilisez la commande suivante :

    ````<html>
      <head>
        <title>Mon projet</title>
      </head>
      <body>
        <h1>Bienvenue sur mon projet !</h1>
      </body>
    </html>```
    ````

5.  Pour afficher le contenu du fichier "index.html", utilisez la commande suivante :
    `cat mon_projet/index.html`
6.  Pour dupliquer le fichier "index.html" et nommer la copie "index_backup.html", utilisez la commande suivante :
    `cp mon_projet/index.html mon_projet/index_backup.html`
7.  Pour afficher le contenu du répertoire "mon_projet", utilisez la commande suivante :
    `ls mon_projet`
8.  Pour renommer le fichier "index_backup.html" en "backup.html", utilisez la commande suivante :
    `mv mon_projet/index_backup.html mon_projet/backup.html`
9.  Pour afficher le contenu du répertoire "mon_projet", utilisez la commande suivante :
    `ls mon_projet`
