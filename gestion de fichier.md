
## Copier des fichiers avec la commande Bash cp

La commande  `cp`  pour “copy” (“copier”) permet de copier des fichiers ou des répertoires dans d’autres fichiers ou répertoires.

Pour copier le contenu d’un fichier dans un autre fichier situé dans le même répertoire, nous écrirons tout simplement  `cp fichier1 fichier2`  où “fichier1” est le fichier à copier et “fichier2” est la copie du fichier. Notez que si “fichier2” n’existe pas avant la copie, il sera crée. Dans le cas contraire, son contenu sera écrasé par le nouveau contenu copié.

Pour copier le contenu d’un fichier dans un autre répertoire, nous utiliserons la syntaxe  `cp fichier1 répertoire1`  où “fichier1” est le fichier à copier et “répertoire1” est le répertoire dans lequel doit être fait la copie. Dans ce cas là, le fichier copié s’appellera également “fichier1”.

Pour copier plusieurs fichiers dans un autre répertoire, nous allons utiliser la syntaxe  `cp fichier1 fichier2 fichier3 répertoire`.

Enfin, la commande  `cp`  va également nous permettre de copier le contenu d’un répertoire dans un autre répertoire. Pour cela, nous allons devoir utiliser l’option  `-R`  de cette commande. Pour copier un répertoire nommé “répertoire1” dans un autre nommé “répertoire2”, nous écrirons  `cp -R répertoire1 répertoire2`. Si “répertoire2” n’existe pas, il sera créé.

Pour tester cette commande, je vous propose de créer un fichier “test.txt” et un dossier “cours” sur votre bureau.

![Utilisation de la commande shell bash cp pour copier des fichiers et des répertoires](https://www.pierre-giraud.com/wp-content/uploads/2019/07/bash-commande-cp-copie-fichier-repertoire.png)

Ici, on commence par  `cd`  vers notre bureau (ligne 1) puis on utilise  `cp`  pour copier notre fichier “test1.txt” en créant une copie nommée “test2.txt” sur le bureau (ligne 2).

Ensuite, on copie “test1.txt” dans notre dossier “cours” (ligne 3) puis on copie finalement les deux fichiers “test1.txt” et “test2.txt” dans ce dossier cours (ligne 4).

Finalement, on effectue une copie de notre répertoire “cours” qu’on appelle “cours-copie” (ligne 5).

## Déplacer ou renommer des fichiers et des répertoires avec la commande Bash mv

La commande  `mv`  pour “move” (“déplacer”) permet de renommer ou de déplacer des fichiers ou des répertoires dans d’autres fichiers ou répertoires.

Pour renommer un fichier ou un répertoire, nous utiliserons la syntaxe  `mv source target`  où “source” est le nom d’origine du fichier ou du répertoire et “target” est le nouveau nom. Si un fichier “target” existe déjà, son contenu sera remplacé par celui de “source”.

Pour déplacer un ou plusieurs fichiers ou répertoires dans un autre répertoire, nous écrirons  `mv source1 source2 répertoire`  où “source1” et “source2” sont les noms de deux fichiers ou de deux répertoires à déplacer et “répertoire” est le nom du répertoire de destination.

![Utilisation de la commande shell bash mv pour renommer ou déplacer des fichiers](https://www.pierre-giraud.com/wp-content/uploads/2019/07/bash-commande-mv-deplacer-renommer-fichier-repertoire.png)

Dans cet exemple, on utilise d’abord  `mv`  pour renommer notre fichier “test1.txt’ en “test.txt” puis on utilise à nouveau  `mv`  pour déplacer ce fichier dans le répertoire “cours”.

## Supprimer des fichiers et des répertoires avec la commande Bash rm

La commande  `rm`  pour “remove” (“supprimer”) permet de supprimer des fichiers ou des répertoires. Attention : tout fichier ou répertoire supprimé avec  `rm`  sera définitivement perdu.

Pour supprimer un ou plusieurs fichiers, on utilisera la syntaxe  `rm fichier`  ou  `rm fichier1 fichier2`.

Pour supprimer un répertoire, il va au préalable falloir supprimer ce qu’il contient ou utiliser une option  `-r`  pour activer la suppression récursive.

![Utilisation de la commande shell bash rm pour supprimer des fichiers ou des répertoires](https://www.pierre-giraud.com/wp-content/uploads/2019/07/bash-commande-rm-supprimer-fichier-repertoire.png)

Ici, on commence par supprimer le fichier “test2.txt” présent sur le bureau. Faites bien attention à  `pwd`  avant pour vous assurer que vous vous situez bien dans le bon répertoire pour ne pas supprimer n’importe quoi !

On tente ensuite de supprimer notre répertoire “cours-copie” avec  `rm`  mais la commande échoue car le répertoire contient des fichiers. On utilise alors  `rm`  avec une option  `-r`  pour vider le répertoire et le supprimer.

## Créer de nouveaux répertoires avec la commande Bash mkdir

La commande  `mkdir`  pour “make directory” (“créer un répertoire”) permet de créer de nouveaux répertoires.

Cette commande est également très simple d’utilisation, il suffit d’écrire  `mkdir répertoire`  pour créer un nouveau répertoire qui portera le nom “répertoire”.

![Utilisation de la commande shell bash mkdir pour créer de nouveaux répertoires](https://www.pierre-giraud.com/wp-content/uploads/2019/07/bash-commande-mkdir-creation-repertoire.png)

On utilise ici la commande  `mkdir`  pour créer un répertoire “Test” sur le bureau.
