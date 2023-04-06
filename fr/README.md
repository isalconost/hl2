# 💻📖 hacker-laws

Lois, théories, principes et modèles que les développeurs trouveront utiles.

[Translations](#translations): [🇮🇩](./translations/id.md) [🇧🇷](./translations/pt-BR.md) [🇨🇳](https://github.com/nusr/hacker-laws-zh) [🇩🇪](./translations/de.md) [🇫🇷](./translations/fr.md) [🇬🇷](./translations/el.md) [🇮🇹](https://github.com/csparpa/hacker-laws-it) [🇱🇻](./translations/lv.md) [🇰🇷](https://github.com/codeanddonuts/hacker-laws-kr) [🇵🇱](./translations/pl.md) [🇷🇺](https://github.com/solarrust/hacker-laws) [🇪🇸](./translations/es-ES.md) [🇹🇷](https://github.com/umutphp/hacker-laws-tr) [🇯🇵](./translations/jp.md) [🇺🇦](./translations/uk.md) [🇻🇳](./translations/vi.md)

Vous aimez ce projet ? S'il vous plaît, envisagez [de me parrainer](https://github.com/sponsors/dwmkerr) ainsi que les [traducteurs](#translations) . Consultez également ce podcast sur [The Changelog - Laws for Hackers to Live By](https://changelog.com/podcast/403) pour en savoir plus sur le projet ! Vous pouvez également [télécharger le dernier eBook PDF](https://github.com/dwmkerr/hacker-laws/releases/latest/download/hacker-laws.pdf) . Consultez le [Guide du contributeur](./.github/contributing.md) si vous souhaitez contribuer !

---

<!-- vim-markdown-toc GFM -->

- [Introduction](#introduction)
- [Lois](#laws)
    - [Principe 90–9–1 (règle du 1 %)](#9091-principle-1-rule)
    - [La loi d'Amdahl](#amdahls-law)
    - [La théorie des fenêtres brisées](#the-broken-windows-theory)
    - [Loi de Brooks](#brooks-law)
    - [Théorème CAP (théorème de Brewer)](#cap-theorem-brewers-theorem)
    - [Les trois lois de Clarke](#clarkes-three-laws)
    - [Loi de Conway](#conways-law)
    - [Loi de Cunningham](#cunninghams-law)
    - [Numéro de Dunbar](#dunbars-number)
    - [L'effet Dunning-Kruger](#the-dunning-kruger-effect)
    - [Loi de Fitts](#fitts-law)
    - [Loi de Gall](#galls-law)
    - [Loi de Goodhart](#goodharts-law)
    - [Rasoir de Hanlon](#hanlons-razor)
    - [Loi de Hick (loi de Hick-Hyman)](#hicks-law-hick-hyman-law)
    - [Loi de Hofstadter](#hofstadters-law)
    - [La loi de Huber](#hutbers-law)
    - [Le cycle de la mode et la loi d'Amara](#the-hype-cycle--amaras-law)
    - [Loi d'Hyrum (La loi des interfaces implicites)](#hyrums-law-the-law-of-implicit-interfaces)
    - [Loi de Kernighan](#kernighans-law)
    - [La loi de Linus](#linuss-law)
    - [Loi de Metcalfe](#metcalfes-law)
    - [la loi de Moore](#moores-law)
    - [Loi de Murphy / Loi de Sod](#murphys-law--sods-law)
    - [Le rasoir d'Occam](#occams-razor)
    - [Loi de Parkinson](#parkinsons-law)
    - [Effet d'optimisation prématuré](#premature-optimization-effect)
    - [Loi de putt](#putts-law)
    - [Loi de Reed](#reeds-law)
    - [La loi de conservation de la complexité (loi de Tesler)](#the-law-of-conservation-of-complexity-teslers-law)
    - [La loi de Déméter](#the-law-of-demeter)
    - [La loi des abstractions qui fuient](#the-law-of-leaky-abstractions)
    - [La loi de l'instrument](#the-law-of-the-instrument)
    - [La loi de la trivialité](#the-law-of-triviality)
    - [La philosophie Unix](#the-unix-philosophy)
    - [La règle scoute](#the-scout-rule)
    - [Le modèle Spotify](#the-spotify-model)
    - [La règle des deux pizzas](#the-two-pizza-rule)
    - [Loi de Wadler](#wadlers-law)
    - [Loi de Wheaton](#wheatons-law)
- [Des principes](#principles)
    - [Tous les modèles sont faux (loi de George Box)](#all-models-are-wrong-george-boxs-law)
    - [Clôture de Chesterton](#chestertons-fence)
    - [L'effet de la mer Morte](#the-dead-sea-effect)
    - [Le principe de Dilbert](#the-dilbert-principle)
    - [Le principe de Pareto (la règle des 80/20)](#the-pareto-principle-the-8020-rule)
    - [Le principe Shirky](#the-shirky-principle)
    - [Le principe de Peter](#the-peter-principle)
    - [Le principe de robustesse (loi de Postel)](#the-robustness-principle-postels-law)
    - [SOLIDE](#solid)
    - [Le principe de responsabilité unique](#the-single-responsibility-principle)
    - [Le principe ouvert/fermé](#the-openclosed-principle)
    - [Le principe de substitution de Liskov](#the-liskov-substitution-principle)
    - [Le principe de ségrégation d'interface](#the-interface-segregation-principle)
    - [Le principe d'inversion de dépendance](#the-dependency-inversion-principle)
    - [Le principe SEC](#the-dry-principle)
    - [Le principe KISS](#the-kiss-principle)
    - [YAGNI](#yagni)
    - [Les erreurs de l'informatique distribuée](#the-fallacies-of-distributed-computing)
    - [Le principe du moindre étonnement](#the-principle-of-least-astonishment)
- [Liste de lecture](#reading-list)
- [Ressources en ligne](#online-resources)
- [Livre électronique PDF](#pdf-ebook)
- [Podcast](#podcast)
- [Traductions](#translations)
- [Projets liés](#related-projects)
- [Contribuant](#contributing)
- [FAIRE](#todo)

<!-- vim-markdown-toc -->

## Introduction

Il y a beaucoup de lois dont les gens discutent lorsqu'ils parlent de développement. Ce référentiel est une référence et un aperçu de certains des plus courants. Veuillez partager et soumettre des PR !

❗ : Ce référentiel contient une explication de certaines lois, principes et modèles, mais ne *préconise* aucun d'entre eux. La question de savoir si elles doivent être appliquées sera toujours un sujet de débat et dépendra grandement de ce sur quoi vous travaillez.

## Lois

Et c'est reparti!

Bonjour, je suis le nouveau paragraphe !!!

### Principe 90–9–1 (règle du 1 %)

[Règle du 1% sur Wikipédia](https://en.wikipedia.org/wiki/1%25_rule_(Internet_culture))

Le principe du 90-9-1 suggère qu'au sein d'une communauté Internet telle qu'un wiki, 90 % des participants ne consomment que du contenu, 9 % éditent ou modifient du contenu et 1 % des participants ajoutent du contenu.

Exemples concrets :

- Une étude réalisée en 2014 sur quatre réseaux sociaux de santé numérique a révélé que les 1 % supérieurs créaient 73 % des publications, les 9 % suivants représentaient une moyenne d'environ 25 % et les 90 % restants représentaient une moyenne de 2 % ( [Référence](https://www.jmir.org/2014/2/e33/) )

Voir également:

- [Principe de Pareto](#the-pareto-principle-the-8020-rule)

### La loi d'Amdahl

[Loi d'Amdahl sur Wikipédia](https://en.wikipedia.org/wiki/Amdahl%27s_law)

> La loi d'Amdahl est une formule qui montre l' *accélération potentielle* d'une tâche de calcul qui peut être obtenue en augmentant les ressources d'un système. Normalement utilisé en calcul parallèle, il permet de prédire le bénéfice réel de l'augmentation du nombre de processeurs, qui est limité par la parallélisabilité du programme.

Mieux illustré par un exemple. Si un programme est composé de deux parties, la partie A, qui doit être exécutée par un seul processeur, et la partie B, qui peut être parallélisée, alors on voit que l'ajout de plusieurs processeurs au système exécutant le programme ne peut avoir qu'un intérêt limité . Cela peut potentiellement améliorer considérablement la vitesse de la partie B - mais la vitesse de la partie A restera inchangée.

Le diagramme ci-dessous montre quelques exemples d'améliorations potentielles de la vitesse :

<img width="480px" alt="Schéma : loi d'Amdahl" src="./images/amdahls_law.png">

*(Référence de l'image : par Daniels219 sur Wikipedia anglais, Creative Commons Attribution-Share Alike 3.0 Unported, https://en.wikipedia.org/wiki/File:AmdahlsLaw.svg)*

Comme on peut le voir, même un programme parallélisable à 50% ne profitera que très peu au-delà de 10 unités de traitement, alors qu'un programme parallélisable à 95% peut encore atteindre des gains de vitesse significatifs avec plus d'un millier d'unités de traitement.

À mesure que [la loi de Moore](#moores-law) ralentit et que l'accélération de la vitesse du processeur individuel ralentit, la parallélisation est essentielle pour améliorer les performances. La programmation graphique est un excellent exemple - avec l'informatique moderne basée sur Shader, des pixels ou des fragments individuels peuvent être rendus en parallèle - c'est pourquoi les cartes graphiques modernes ont souvent plusieurs milliers de cœurs de traitement (GPU ou Shader Units).

Voir également:

- [Loi de Brooks](#brooks-law)
- [la loi de Moore](#moores-law)

### La théorie des fenêtres cassées

[La théorie des fenêtres cassées sur Wikipedia](https://en.wikipedia.org/wiki/Broken_windows_theory)

La théorie des fenêtres brisées suggère que les signes visibles de crime (ou le manque de soin d'un environnement) conduisent à d'autres crimes plus graves (ou à une détérioration supplémentaire de l'environnement).

Cette théorie a été appliquée au développement de logiciels, suggérant qu'un code de mauvaise qualité (ou [dette technique](#TODO) ) peut conduire à la perception que les efforts pour améliorer la qualité peuvent être ignorés ou sous-évalués, conduisant ainsi à un code de mauvaise qualité supplémentaire. Cet effet se répercute en cascade, entraînant une forte diminution de la qualité au fil du temps.

Voir également:

- [Dette technique](#TODO)

Exemples:

- [La programmation pragmatique : l'entropie logicielle](https://flylib.com/books/en/1.315.1.15/1/)
- [Coder l'horreur : la théorie de la fenêtre brisée](https://blog.codinghorror.com/the-broken-window-theory/)
- [OpenSource : Joie de programmer - La théorie de la fenêtre brisée](https://opensourceforu.com/2011/05/joy-of-programming-broken-window-theory/)
