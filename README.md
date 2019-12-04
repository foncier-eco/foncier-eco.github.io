_Le [dépôt principal][depot] du projet est sur Gitlab. Merci de déposer vos remarques et propositions de fusion à cet endroit_.

# Foncier Economique
Initié dans le cadre de plusieurs réflexions coordonnées sur le foncier et l'activité économique, ce site sert de support et de démonstrateur au [collectif foncier](./docs/a_propos/partenaires.md) pour mettre à disposition des ressources utiles aux acteurs dans ce domaine.

## Contribuer
Le projet se veut ouvert aux commentaires et aux [contributions](./docs/a_propos/contribuer.md).

## Tester foncier-eco sur votre machine

L'outil nécessite [python][python] 3.x pour produire les pages ainsi que les bibliothèques figurant dans [py-requirements.txt](py-requirements.txt). Une fois python installé, on peut les installer facilement en faisant
```bash
pip install -r py-requirements.txt
```

Ceci fait, on peut lancer un serveur virtuel qui permet à la fois de prévisualiser le site, mais de visualiser en temps réel les modification qu'on fait dans le projet.
```bash
mkdocs serve
```

On peut également produire l'ensemble du site tel qu'il sera envoyé au serveur. Le résultat apparaitra dans un dossier `site` . Une fois les pages produites, le site est "statique" et ne nécessite rien d'autre qu'un serveur de fichiers.
```bash
mkdocs build
```

### problèmes divers
En fonction des versions de _python_ il est possible que l'installation ou la mise en place du serveur virtuel fasse émerger quelques accrocs. Nous essayons de tenir à jour des solutions à ce sujet sur le site d'un autre projet qui utilise la même _motorisation_.

## Licences

Foncier Eco est libre et s'appuye sur des logiciels libres

* [MkDocs][mkdocs] propulse le wiki - licence BSD 2-Clause
  * le theme [material][material] - licence MIT
  * le plugin [awesome-pages][awesome] - licence MIT

L'ensemble des adaptations, développements et contenus sont, sauf mention contraire, sous [licence ouverte](./LICENCE.md)

[depot]: https://gitlab.com/foncier-eco/foncier-eco.gitlab.io
[mkdocs]: https://www.mkdocs.org
[material]: https://squidfunk.github.io/mkdocs-material
[python]: https://www.python.org/
