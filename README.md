# Installation

Les thèmes de ce projet fonctionnent grâce à Betterdiscord. Betterdiscord est un programme permettant d'étendre les fonctionnalités du client classique grâce notamment à des plugins (possibilité de citer des messages, de crypter des conversation, etc.) et des thèmes (comme ce projet).

Si vous ne l'avez pas encore installé sur votre système, je vous conseille de télécharger et installer Betterdiscord, et plus particulièrement le fork que Rauenzi a fait de ce logiciel, disponible [ici](https://github.com/rauenzi/BetterDiscordApp/releases). _BandageBD_ est compatible avec les systèmes Windows et MacOS nativement. Pour les utilisateurs Linux, vous devrez vous débrouiller avec l'archive `.tar.gz` ou alors, si vous avez de la chance, votre gestionnaire de paquet l'aura intégré dans ses dépôts.

Une fois _BandageBD_ installé, rechargez Discord (`ctrl + R` sous Windows et Linux) afin qu'il prenne en compte les changements de configuration. Pour savoir si le programme a été détecté, ouvrez les paramètres de Discord : une nouvelle section intitulée `Bandaged BD` doit s'être ajoutée à la liste de paramètres existante. Si ce n'est pas le cas, redémarrez Discord jusqu'à ce que ça apparaisse, ou alors réinstallez _Bandaged BD_.

Pout installer le(s) thème(s) de votre choix, il vous suffit de télécharger les fichiers de votre choix ayant l'extension `.theme.css`. Ceci fait, rendez-vous dans les paramètres de Discord, dans la section _Themes_ et cliquez sur le bouton _Open Theme Folder_. Collez-y le(s) thème(s) que vous avez téléchargés.

Pour activer/désactiver un thème, il vous suffit de cliquer sur le bouton prévu à cet effet à côté du nom de chacun. Une fois un thème activé, l'interface de Discord devrait changer automatiquement afin de s'adapter à la nouvelle configuration.

# Personnaliser un thème existant

Le thème de base (pas très beau, je vous l'accorde 😉) est `nadt.theme.css`.

Les thèmes fournis dans ce projet ne sont pas à votre goût ? Pas de soucis, la personnalisation est très simple.

Pour commencer, ouvrez les paramètres de Discord et rendez-vous dans la section _Custom CSS_.

## Changer l'apparence générale (couleurs, police d'écriture, etc.)

1. `--mainColor: <couleur>` : permet notamment de changer la couleur des titres, de l'intitulé des boutons, des checkboxes, l'arrière-plan des noms de serveurs (s'ils n'ont pas d'avatar), ainsi que celui des notifications.
2. `--secondColor: <couleur>` : permet notamment de modifier l'arrière plan des boutons et le style appliqué aux noms des serveurs lorsqu'ils sont survolés.
3. `--thirdColor: <couleur>` : modifie la couleur d'arrière-plan des salons de discussion, de la liste d'amis, de la liste des membres d'un serveur ou encore celui des paramètres.
4. `--font: <nom_police>` : change la police de caractère utilisée par Discord. Cette règle est à utiliser conjointement avec `@import url(<url_police>)`. Cette règle est détaillée au point suivant.
5. `--textColor: <couleur>` : change la couleur du texte (presque) partout dans Discord.

Toutes ces règles (à l'exception du `@import` qui doit être placé en premier, en-dehors de tout ensemble de règles) doivent être placées à l'intérieur d'un bloc de déclarations comme suit :

    :root {
        règle1 : <valeur>;
        règle2 : <valeur>;
        }

## Changer la police d'écriture

C'est un peu plus compliqué... 😁 Vous devez d'abord connaître la police que vous désirez utiliser. Ensuite, vérifier si elle est disponible via [Google fonts](https://fonts.google.com) [ou un équivalent](https://alternativeto.net/software/google-web-fonts/).

Ceci fait, vous pouvez importer la police à utiliser grâce à une règle à entrer  dans la boîte de saisie _Custom CSS_, comme ceci :

    `@import url(<url_police>);`

    :root {
        --font : <nom_police>;
    }

N'oubliez pas non plus d'utiliser le paramètre `--font: <nom_police> !important` afin d'utiliser la police dans votre thème.

Vous pouvez changer le couleur du texte grâce à la règle `--textColor: <couleur>`.

## Modifier la couleur/l'image utilisée en fond d'écran de Discord

Vous pouvez utiliser le schéma suivant :

    body {
        background-image: url(<url_image>);
        background-color: <couleur>;
    }
    
Notez que vous ne pouvez appliquer que l'une de ces deux règles, et non pas les deux en même temps.

# Contribuer

Vous pouvez contribuer à ce projet en proposant des améliorations (ouvrir une issue, une pull request, ...) ou me contactant par mail ou via Diaspora.

# Un problème, une question ?

Ouvrez une issue ou contactez-moi si vous avez le moindre problème et que vous ne savez pas comment le régler par vous-même.

# Licence

L'entiéreté de ce dépôt est placé sous licence GNU GPL v3, à l'exception de l'avatar du projet, qui vient d'[ici](https://www.iconfinder.com/icons/1542372/discord_media_social_icon).

