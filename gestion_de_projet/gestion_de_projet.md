# Gestion des droits d'accès

## Windows

Sur Windows, les droits d'accès sont gérés à l'aide de groupes d'utilisateurs et de permissions. Les groupes d'utilisateurs permettent de regrouper des utilisateurs en fonction de leurs besoins d'accès. Les permissions déterminent les actions que les utilisateurs sont autorisés à effectuer sur les fichiers, les dossiers et les autres ressources.

Il existe plusieurs types de permissions dans Windows, tels que la lecture, l'écriture, l'exécution et la modification. Les permissions peuvent être accordées au niveau du groupe ou de l'utilisateur, et peuvent être définies pour des fichiers, des dossiers ou même des disques entiers.

Vous pouvez modifier les permissions à l'aide de l'interface graphique ou en utilisant la commande icacls dans l'invite de commande. Par exemple, pour donner l'autorisation à un utilisateur nommé "Alice" de modifier un dossier nommé "Documents", vous pouvez utiliser la commande suivante :

```
icacls "C:\Users\Alice\Documents" /grant Alice:(M)
```

### Exercice

Vous avez un dossier nommé "Projets" qui contient plusieurs sous-dossiers et fichiers. Vous souhaitez accorder les permissions suivantes :

-   Le groupe "Développeurs" doit avoir un accès complet (lecture, écriture, modification et suppression) à tous les fichiers et sous-dossiers de "Projets".
-   Le groupe "Utilisateurs" doit avoir un accès en lecture seule à tous les fichiers et sous-dossiers de "Projets", mais ne doit pas être autorisé à modifier ou supprimer quoi que ce soit.

Comment pouvez-vous mettre en place ces permissions ?

## macOS

Sur macOS, les droits d'accès sont gérés à l'aide de la fonctionnalité de contrôle des accès de base (BAC, pour Basic Access Control). Le BAC est basé sur les listes de contrôle d'accès (ACL, pour Access Control Lists) et permet de définir des règles pour les fichiers et les dossiers.

Les ACL permettent de spécifier les utilisateurs et les groupes autorisés à accéder à une ressource, ainsi que les types d'accès autorisés, tels que la lecture, l'écriture et l'exécution. Les ACL peuvent également être hiérarchiques, ce qui permet de définir des règles pour les dossiers et les sous-dossiers.

Vous pouvez modifier les ACL en utilisant la commande chmod. Par exemple, pour donner l'autorisation à un utilisateur nommé "Bob" de lire et d'écrire un fichier nommé "notes.txt", vous pouvez utiliser la commande suivante :

```
chmod +a "Bob allow read,write" notes.txt
```

### Exercice

Vous avez un dossier nommé "Photos" qui contient des fichiers et des sous-dossiers de photos. Vous souhaitez accorder les permissions suivantes :

-   L'utilisateur "Alice" doit avoir un accès complet à tous les fichiers et sous-dossiers de "Photos".
-   L'utilisateur "Bob" doit avoir un accès en lecture seule à tous les fichiers et sous-dossiers de "Photos".

Comment pouvez-vous mettre en place ces permissions en utilisant les ACL ?

## Linux

Sur Linux, les droits d'accès sont gérés à l'aide de la commande chmod, qui permet de modifier les permissions sur les fichiers et les dossiers. Les permissions sont divisées en trois catégories : propriétaire, groupe et autres.

La commande chmod utilise des chiffres pour spécifier les permissions. Les chiffres 4, 2 et 1 représentent respectivement les permissions de lecture, écriture et exécution. Les chiffres sont ensuite combinés pour définir les permissions pour le propriétaire, le groupe et les autres.

### Changer les droits avec la commande chmod

La commande `chmod` (change mode) est utilisée pour modifier les droits d'accès d'un fichier ou d'un dossier.

La syntaxe de la commande `chmod` est la suivante :

`chmod options mode file/directory` 

-   `options` : options facultatives de la commande.
-   `mode` : définit les nouveaux droits d'accès. Il peut être défini de plusieurs manières :
    -   Notation octale : un chiffre de 0 à 7 pour chaque groupe d'utilisateurs (propriétaire, groupe, autres). Chaque chiffre correspond à une combinaison binaire de 3 bits qui définit les droits de lecture, d'écriture et d'exécution. Par exemple, `chmod 644 fichier` donnera les droits de lecture et d'écriture au propriétaire du fichier, et le droit de lecture pour le groupe et les autres.
    -   Notation symbolique : une lettre (u pour le propriétaire, g pour le groupe, o pour les autres, a pour tous les utilisateurs) suivie d'un opérateur (+ pour ajouter des droits, - pour retirer des droits, = pour définir des droits précis), suivi d'une lettre (r pour la lecture, w pour l'écriture, x pour l'exécution). Par exemple, `chmod u+x fichier` donnera le droit d'exécution au propriétaire du fichier.
-   `file/directory` : nom du fichier ou du dossier sur lequel appliquer les modifications.

Voici quelques exemples d'utilisation de la commande `chmod` :

#### Donne les droits de lecture et d'écriture au propriétaire, et le droit de lecture pour le groupe et les autres.
```
chmod 644 fichier.txt
```
#### Donne les droits d'exécution au propriétaire et au groupe.
```
chmod ug+x script.sh
```
#### Retire le droit d'écriture pour tous les utilisateurs.
```
chmod a-w fichier.txt` 
```
### Changer les droits avec la commande chown

La commande `chown` (change owner) est utilisée pour changer le propriétaire d'un fichier ou d'un dossier.

La syntaxe de la commande `chown` est la suivante :

`chown options user:group file/directory`

-   `options` : options facultatives de la commande.
-   `user` : nom d'utilisateur ou UID du nouveau propriétaire.
-   `group` : nom de groupe ou GID du nouveau groupe.
-   `file/directory` : nom du fichier ou du dossier sur lequel appliquer les modifications.

Voici quelques exemples d'utilisation de la commande `chown` :

#### Change le propriétaire et le groupe du fichier.
```
chown utilisateur:groupe fichier.txt
```
#### Change le propriétaire du dossier et de son contenu récursivement.
```
chown -R utilisateur dossier/` 
```
## Changer les droits avec la commande chgrp

La commande `chgrp` (change group) est utilisée pour changer le groupe d'un fichier ou d'un dossier.

La syntaxe de la commande `chgrp` est la suivante :

`chgrp options group file/directory` 

-   `options` : options facultatives de la commande.
-   `group` : nom de groupe ou GID du nouveau groupe.
-   `file/directory` : nom du fichier ou du dossier sur lequel appliquer le
Pour modifier les droits avec la commande `chgrp`, vous devez utiliser l'une des options suivantes :

-   `-R` : applique la modification de groupe récursivement à tous les fichiers et sous-dossiers du dossier spécifié.
-   `--reference` : copie les permissions de groupe d'un fichier ou d'un dossier spécifié sur un autre fichier ou dossier.

Voici quelques exemples d'utilisation de la commande `chgrp` :

#### Change le groupe du fichier
```
chgrp groupe fichier.txt
```
#### Change le groupe du dossier et de son contenu récursivement
```
chgrp -R groupe dossier/
```
#### Copie les permissions de groupe du fichier source vers le fichier de destination
```
chgrp --reference=fichier-source fichier-destination` 
```
Notez que pour utiliser la commande `chgrp`, vous devez être propriétaire du fichier ou du dossier ou disposer de privilèges d'administration (en tant que super-utilisateur ou avec la commande `sudo`).

### Exercice

Vous avez un fichier nommé "rapport.txt" qui contient des informations sensibles. Vous souhaitez accorder les permissions suivantes :

-   Le propriétaire du fichier doit avoir un accès complet (lecture, écriture et exécution) au fichier.
-   Les membres du groupe "Finances" doivent avoir un accès en lecture seule au fichier.
-   Tous les autres utilisateurs ne doivent pas avoir d'accès au fichier.

Comment pouvez-vous mettre en place ces permissions en utilisant la commande chmod ?

## Conclusion

La gestion des droits d'accès est une partie essentielle de la sécurité informatique. Les différents systèmes d'exploitation ont leur propre manière de gérer les droits d'accès, mais ils ont tous un objectif commun : protéger les données et les ressources sensibles du système. En comprenant comment les droits d'accès sont gérés sur votre système d'exploitation, vous pouvez mieux protéger vos données et votre système contre les menaces potentielles.