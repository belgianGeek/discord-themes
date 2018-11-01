Ce projet a pour but de permettre à toute personnne de personnaliser l'interface de Discord selon ses envies (couleurs, fond d'écran, police, etc.) et se veut utilisable par tous, sans avoir nécessairement des compétences/connaissances en programmation.

# Installation

Les thèmes de ce projet fonctionnent grâce à Betterdiscord. Betterdiscord est un programme permettant d'étendre les fonctionnalités du client classique grâce notamment à des plugins (possibilité de citer des messages, de crypter des conversation, etc.) et des thèmes (comme ce projet).

Si vous ne l'avez pas encore installé sur votre système, je vous conseille de télécharger et installer Betterdiscord, et plus particulièrement de fork que Rauenzi a fait de ce logiciel, disponible [ici](https://github.com/rauenzi/BetterDiscordApp/releases). _BandageBD_ est compatible avec les systèmes Windows et Linux nativement. Pour les utilisateurs Linux, vous devrez vous débrouiller avec l'archive `.tar.gz` ou alors, si vous avez de la chance, votre gestionnaire de paquet l'aura intégré dans ses dépôts.

Une fois _BandageBD_ installé, rechargez Discord (`ctrl + R` sous Windows et Linux) afin qu'il prenne en compte les changements de configuration. Pour savoir si le programme a été détecté, ouvrez les paramètres de Discord : une nouvelle section intitulée `Bandaged BD` doit s'être ajoutée à la liste de paramètres existante. Si ce n'est pas le cas, redémarrez Discord jusqu'à ce que ça apparaisse, ou alors réinstallez _Bandaged BD_.

Pout installer le(s) thème(s) de votre choix, il vous suffit de télécharger les fichiers de votre choix ayant l'extension `.theme.css`. Ceci fait, rendez-vous dans les paramètres de Discord, dans la section _Themes_ et cliquez sur le bouton _Open Theme Folder_. Collez-y le(s) thème(s) que vous avez téléchargés.

Pour activer/désactiver un thème, il vous suffit de cliquer sur le bouton prévu à cet effet à côté du nom de chacun. Une fois un thème activé, l'interface de Discord devrait changer automatiquement afin de s'adapter à la nouvelle configuration.

# Personnaliser un thème existant

Le thème de base (pas très beau, je vous l'accorde 😉) est `nadt.theme.css`.

Les thèmes fournis dans ce projet ne sont pas à votre goût ? Pas de soucis, la personnalisation est très simple:

- Ouvrez les paramètres de Discord et rendez-vous dans la section _Custom CSS_.
- Pour changer les couleurs, commencez par taper ceci dans la boîte de saisie, en remplaçant _couleur1_, _couleur2_ et _couleur3_ par ce que vous désirez.

    ![changer les couleurs de Discord](https://framapic.org/V2lfjDN5nHH5/ytHmpDrFxAZP.png)

- Pour changer le fond d'écran, il vous suffit d'ajouter ces règles-ci dans la même boîte de saisie :

    ![changer le fond d'écran de Discord](https://framapic.org/YoO6zOI5vZn4/ZQh4LmjGm1hH.png)

- Changer la police d'écriture est un peu plus compliqué... 😁 Vous devez d'abord connaître la police que vous désirez utiliser. Ensuite, vérifier si elle est disponible via [Google fonts](https://fonts.google.com) [ou un équivalent](https://alternativeto.net/software/google-web-fonts/).

Ceci fait, vous pouvez importer la police à utiliser grâce à une règle à entrer  dans la boîte de saisie _Custom CSS_, comme ceci :

    ![changer la police de Discord](https://framapic.org/8sVtya3xxhF3/bCJvNi42EqxB.png)

N'oubliez pas non plus d'utiliser le paramètre `--font: <nom_police> !important` afin d'utiliser la police dans votre thème.

Vous pouvez changer le couleur du texte grâce à la règle `--textColor: <couleur>`.

# Contribuer

Vous pouvez contribuer à ce projet en proposant des améliorations (ouvrir une issue, une pull request, ...) ou me contactant par mail ou via Diaspora.

# Un problème, une question ?

Ouvrez une issue ou contactez-moi si vous avez le moindre problème et que vous ne savez pas comment le régler par vous-même.

# Licence

L'entiéreté de ce dépôt est placé sous licence GNU GPL v3, à l'exception de l'avatar du projet, qui vient d'[ici](https://www.iconfinder.com/icons/1542372/discord_media_social_icon).

