title: Contribuer directement au code

_Les éléments présentés ici pourront paraitre technique pour les personnes qui n'ont jamais utilisé un outil de gestion de version. Un peu de pratique suffit pour constater qu'il n'en est rien. Toutefois nous proposons d'autres possibilités pour [contribuer](../contribuer.md) à ceux que cela effraierait trop_

Le prérequis indispensable pour les méthodes présentées ici est de disposer d'un compte sur gitlab ou github.

## Créez votre _fork_

* Rendez vous sur le dépôt du projet sur la plate-forme de votre choix :
    * [Gitlab][gitlab] (de préférence)
    * [Github][github]
* Cliquez sur le bouton ''Fork'' et suivez les instructions pour ajouter ce projet à vos projets ou à ceux de votre organisation.

La plate-forme vient de vous créer une version du projet pour vous à l'adresse `https://gitlab.com/votre_identifiant/nom_de_votre_projet`. Elle reste liée au projet principal et vous permettra de soumettre vos modifications le moment venu.

## Ajoutez, modifiez, enlevez

Sur cette version du projet qui est la vôtre, vous pouvez faire toutes les modifications (et tous les tests) que vous souhaitez.

### Directement en ligne sur les plate-formes
Les deux plate-formes proposent des éditeurs de texte en ligne qui permettent de faire des modifications, ajouter des fiches, ou en supprimer.

A chaque modification, vous créerez un _commit_ qui fera état des modifications intervenues.

Pour l'instant, avec cette méthode vous pourrez avoir une idée de ce que donneront vos modifications à travers la prévisualisation des fichiers. Sous Gitlab, à chaque commit sur votre branche master, sera générée une version plus ou moins fonctionnelle du site à l'adresse `https://votre_identifiant.gitlab.io/nom_de_votre_projet`

### Sur votre poste de travail

#### Installations et préparation
Le wiki utilise [mkdocs][mkdocs] avec un certain nombre d'extensions. Il vous faudra donc préparer votre poste pour travailler dessus :

* Installez un [client git][git-clients] pour récupérer les données de votre dépôt et envoyer vos modifications[^1];
* Installez [python][python] en version 3.x - Pypy doit fonctionner aussi;
* Installez mkdocs et les extensions requises :

```bash
pip install -r py-requirements.txt
```

* Créez une copie locale de votre dépôt pour travailler.
* Le cas échéant, placez vous via git sur une branche de travail de votre choix.
* Vous pouvez tester votre installation
    * Lancez un terminal
    * Placez vous dans votre répertoire de travail `cd votre_repertoire`
    * Lancez mkDocs `mkdocs serve`
    * Rendez vous dans votre navigateur à l'adresse https://127.0.0.1:8000

#### Modifications
Vous pouvez travailler que le serveur soit lancé ou pas.  L'édition des pages du site se fait dans un éditeur de texte classique. Si le serveur est en route, vos modifications apparaitrons sur votre site de démonstration dès sauvegarde.

#### Sauvegardes, Envois
Lorsque vous êtes satisfaits des modifications effectuées, vous créez un nouveau commit sur votre branche de travail. Pensez à bien indiquer les principales modifications effectuées.

Poussez vos modifications sur votre dépôt.

#### Problèmes dans l'exécution du programme
Il est possible que le programme soit un peu capricieux, au moment de l'installation (problèmes de dépendances, de connexion etc.) ou durant son exécution. Le même programme étant utilisé sur un autre projet, nous essayons de tenir à jour une liste des difficultés rencontrées et des solutions associées : [Problèmes fréquents avec mkdocs](https://gitlab.com/know-rmandie/know-rmandie.gitlab.io/issues/5)

## Envoyez vos propositions
Vous pouvez ensuite faire une demande d'intégration de vos corrections au dépôt principal (_merge request_ ou _pull request_) depuis le site internet de la plate-forme.

Les demandes de fusion sont à faire sur la branche **contributions**.


[^1]: Nous utilisons [tortoise git][tortoise] et [fork][fork], mais nous le disons juste pour ceux qui auraient du mal à choisir. Il y a plein de très bons [clients git][git-clients].

[git-clients]: https://git-scm.com/downloads/guis
[mkdocs]: https://www.mkdocs.org/
[python]: https://www.python.org/
[tortoise]: https://tortoisegit.org/
[fork]: https://git-fork.com/
[gitlab]: https://gitlab.com/
[github]: https://github.com/
