
# Quels sont les différents types de shells sous Linux ?

Publié le 3 août 2022

-   [UNIX/Linux](https://www.digitalocean.com/community/tags/unix-linux "UNIX/Linux")

![Avatar par défaut](https://doimages.nyc3.digitaloceanspaces.com/46f22fba-7718-478b-86ae-e8b875f0473e_default-avatar.jpeg)

Par [nina](https://www.digitalocean.com/community/users/ninad)[](https://www.digitalocean.com/community/users/ninad)

![Quels sont les différents types de shells sous Linux ?](https://journaldev.nyc3.digitaloceanspaces.com/2020/04/Different-types-of-shells.png "Quels sont les différents types de shells sous Linux ?")

Bien que nous pensions que ce contenu profite à notre communauté, nous ne l'avons pas encore examiné en profondeur. Si vous avez des suggestions d'améliorations, n'hésitez pas à nous en faire part en cliquant sur le bouton "Signaler un problème" en bas du didacticiel.

Les shells sont une partie importante de toute session utilisateur Linux. Nous disposons de plusieurs types de shells différents sous Linux pour accomplir des tâches. Chaque coquille a des propriétés uniques. Par conséquent, il existe de nombreux cas où un shell est meilleur que l'autre pour des besoins spécifiques.

Il est donc important pour nous de connaître les différents types de shells disponibles sous Linux. Dans ce tutoriel, nous discuterons de ce qu'est un shell et pourquoi est-ce important.

De plus, nous explorerons différents types de shells sous Linux pour comprendre leurs fonctions et leurs propriétés.

## [Qu'est-ce qu'un Shell et pourquoi en avons-nous besoin ?](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#what-is-a-shell-and-why-do-we-need-them)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#what-is-a-shell-and-why-do-we-need-them)

Chaque fois qu'un utilisateur se connecte au système ou ouvre une fenêtre de console, le noyau exécute une nouvelle instance de shell. Le noyau est le cœur de tout système d'exploitation.

Il est responsable de la gestion des contrôles, de l'exécution des processus et de la bonne utilisation des ressources système.

Un shell est un programme qui agit comme une interface entre un utilisateur et le noyau. Il permet à un utilisateur de donner des commandes au noyau et de recevoir des réponses de celui-ci. Grâce à un shell, nous pouvons exécuter des programmes et des utilitaires sur le noyau. Par conséquent, à la base, un shell est un programme utilisé pour exécuter d'autres programmes sur notre système.

Pouvoir interagir avec le noyau fait des shells un outil puissant. Sans la possibilité d'interagir avec le noyau, un utilisateur ne peut pas accéder aux utilitaires offerts par le système d'exploitation de sa machine.

Comprenons les principaux shells disponibles pour l'environnement Linux.

## [Différents types de shells sous Linux](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#different-types-of-shells-in-linux)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#different-types-of-shells-in-linux)

Si vous comprenez maintenant ce qu'est un noyau, ce qu'est un shell et pourquoi un shell est si important pour les systèmes Linux, passons à l'apprentissage des différents types de shells disponibles.

Chacune de ces coques a des propriétés qui les rendent très efficaces pour un type d'utilisation spécifique par rapport aux autres coques. Discutons donc des différents types de shells sous Linux ainsi que de leurs propriétés et fonctionnalités.

### [1. Le](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#1-the-bourne-shell-https-en-wikipedia-org-wiki-bourne_shell-sh) [Bourne Shell](https://en.wikipedia.org/wiki/Bourne_shell) (sh)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#1-the-bourne-shell-https-en-wikipedia-org-wiki-bourne_shell-sh)

Développé à AT&T Bell Labs par Steve Bourne, le shell Bourne est considéré comme le premier shell UNIX de tous les temps. Il est noté sh. Il a gagné en popularité en raison de sa nature compacte et de sa vitesse de fonctionnement élevée.

C'est ce qui en a fait le shell par défaut du système d'exploitation Solaris. Il est également utilisé comme shell par défaut pour tous les scripts d'administration du système Solaris. Commencez à lire sur [les scripts shell ici](https://www.digitalocean.com/community/tutorials/arrays-in-shell-scripts) .

**Cependant, le shell Bourne présente des inconvénients majeurs.**

-   Il n'a pas de fonctionnalité intégrée pour gérer les opérations logiques et arithmétiques.
-   De plus, contrairement à la plupart des différents types de shells sous Linux, le shell Bourne ne peut pas rappeler les commandes précédemment utilisées.
-   Il manque également des fonctionnalités complètes pour offrir une utilisation interactive correcte.

Le chemin d'accès complet pour le shell Bourne est /bin/sh et /sbin/sh. Par défaut, il utilise l'invite _#_ pour l'utilisateur root et _$_ pour les utilisateurs non root.

### [2. Le](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#2-the-gnu-bourne-again-shell-https-www-gnu-org-software-bash-bash) [shell GNU Bourne-Again](https://www.gnu.org/software/bash/) (bash)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#2-the-gnu-bourne-again-shell-https-www-gnu-org-software-bash-bash)

Plus connu sous le nom de shell Bash, le shell GNU Bourne-Again a été conçu pour être compatible avec le shell Bourne. Il intègre des fonctionnalités utiles de différents types de shells sous Linux, tels que le shell Korn et le shell C.

Il nous permet de rappeler automatiquement les commandes précédemment utilisées et de les modifier à l'aide des touches fléchées, contrairement au shell Bourne.

Le nom de chemin complet pour le shell GNU Bourne-Again est /bin/bash. Par défaut, il utilise l'invite _bash-VersionNumber#_ pour l'utilisateur root et _bash-VersionNumber$_ pour les utilisateurs non root.

### [3. Le](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#3-the-c-shell-http-bxr-su-netbsd-bin-csh-csh) [shell C](http://bxr.su/NetBSD/bin/csh/) (csh)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#3-the-c-shell-http-bxr-su-netbsd-bin-csh-csh)

Le shell C a été créé à l'Université de Californie par Bill Joy. Il est noté csh. Il a été développé pour inclure des fonctionnalités de programmation utiles telles que la prise en charge intégrée des opérations arithmétiques et une syntaxe similaire au langage de programmation C.

De plus, il incorporait l'historique des commandes qui manquait dans différents types de shells sous Linux comme le shell Bourne. Une autre caractéristique importante d'un shell C est les "alias".

Le nom de chemin complet pour le shell C est /bin/csh. Par défaut, il utilise l'invite _hostname#_ pour l'utilisateur root et _hostname%_ pour les utilisateurs non root.

### [4. Le](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#4-the-korn-shell-http-www-kornshell-com-ksh) [coquillage Korn](http://www.kornshell.com/) (ksh)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#4-the-korn-shell-http-www-kornshell-com-ksh)

Le shell Korn a été développé chez AT&T Bell Labs par David Korn, pour améliorer le shell Bourne. Il est noté ksh. Le shell Korn est essentiellement un sur-ensemble du shell Bourne.

En plus de prendre en charge tout ce qui serait pris en charge par le shell Bourne, il offre aux utilisateurs de nouvelles fonctionnalités. Il permet une prise en charge intégrée des opérations arithmétiques tout en offrant des fonctionnalités interactives similaires au shell C.

Le shell Korn exécute des scripts conçus pour le shell Bourne, tout en offrant une manipulation de chaînes, de tableaux et de fonctions similaire au langage de programmation C. Il prend également en charge les scripts écrits pour le shell C. De plus, il est plus rapide que la plupart des différents types de shells sous Linux, y compris le shell C.

Le nom de chemin complet pour le shell Korn est /bin/ksh. Par défaut, il utilise l'invite _#_ pour l'utilisateur root et _$_ pour les utilisateurs non root.

### [5. Le](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#5-the-z-shell-https-ohmyz-sh-zsh) [shell Z](https://ohmyz.sh/) (zsh)[](https://www.digitalocean.com/community/tutorials/different-types-of-shells-in-linux#5-the-z-shell-https-ohmyz-sh-zsh)

Le Z Shell ou zsh est une extension de shell sh avec des tonnes d'améliorations pour la personnalisation. Si vous voulez un shell moderne qui possède toutes les fonctionnalités bien plus, le shell zsh est ce que vous recherchez.

**Certaines caractéristiques remarquables du shell z incluent :**

-   Générer des noms de fichiers en fonction de conditions données
-   Prise en charge des plugins et des thèmes
-   Index des fonctions intégrées
-   Achèvement de la commande
-   et beaucoup plus…

Résumons les différents shells sous Linux dont nous avons parlé dans ce tutoriel dans le tableau ci-dessous.

**Coquille**

**Chemin d'accès complet**

**Invite pour l'utilisateur root**

**Invite pour l'utilisateur non root**

coquille Bourne (sh)

/bin/sh et /sbin/sh

#

$

Shell GNU Bourne-Again (bash)

/bin/bash

bash-VersionNumber#

bash-VersionNumber$

Coquille C (csh)

/bin/csh

#

%

Coquille de Korn (ksh)

/bin/ksh

#

$

Coque Z (zsh)

/bin/zsh

<nom d'hôte>#

<nom d'hôte> 
