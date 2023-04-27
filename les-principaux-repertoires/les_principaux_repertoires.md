# Présentation des différents répertoires en Shell

En Shell, les répertoires sont des emplacements physiques sur le système de fichiers où les fichiers et les dossiers peuvent être stockés. Ils sont organisés dans une hiérarchie arborescente et peuvent être navigués en utilisant des commandes telles que cd, ls et pwd.

## Voici les principaux répertoires en Shell :

- Répertoire racine: Le répertoire de niveau supérieur dans la hiérarchie des fichiers du système de fichiers. Il est représenté par le symbole / et contient tous les autres répertoires et fichiers du système.
- Répertoire personnel: Le répertoire de l'utilisateur actuel. Il est représenté par le symbole ~ et peut être accédé en tapant cd ~ ou simplement cd.
- Répertoire courant: Le répertoire actuel dans lequel se trouve l'utilisateur. Il peut être obtenu en tapant pwd.
- Répertoire parent: Le répertoire supérieur du répertoire courant. Il peut être représenté par le symbole .. et peut être accédé en tapant cd ...
- Répertoire temporaire: Le répertoire dans lequel les fichiers temporaires sont stockés. Il est généralement situé dans /tmp.

En plus de ces répertoires, il existe d'autres répertoires importants en fonction du système d'exploitation, tels que le répertoire bin qui contient les fichiers binaires des programmes, le répertoire etc qui contient les fichiers de configuration du système, et le répertoire var qui contient les fichiers variables du système.

## Exercice 1

- Naviguez jusqu'au répertoire var en utilisant la commande cd.

```
sh
Copy code
cd /var
```

## Exercice 2

- Affichez le contenu du répertoire personnel de l'utilisateur courant.

```
sh
Copy code
ls ~
```

En utilisant les répertoires Shell, vous pouvez naviguer facilement dans la hiérarchie des fichiers du système de fichiers et accéder aux fichiers et dossiers dont vous avez besoin. Il est important de comprendre ces répertoires et comment les utiliser pour effectuer des tâches de gestion de fichiers courantes en Shell.
