# Tester plusieurs versions de node dans un workflow

## Comment exécuter ?

Il suffit d'activer le trigger de l'action à savoir un "push". 

Cependant pour push il faut pouvoir avoir un commit.

Vous connaissez peut être les "dummy commit" qui sont des modifications mineurs, un espace par ci, juste pour pouvoir créer un commit.


Mais ici, on fait les choses proprement pourquoi faire un faux commit quand on peut faire un commit vide ?!

```bash
git commit --allow-empty -m "Commit totalement vide !"
```

Il suffit alors de push tout ça vers Github

```bash
git push
```

Il reste à aller voir l'interface de Github pour observer le résultat dans les actions.

## Ou trouvez le script ?
[la définition de l'action](./.github/workflows/multi-node.yaml)

## Formation sur GitHub Actions

Ce projet fait partit d'une formation sur l'utilisation de GitHub Actions et découvrir comment automatiser vos intégrations continues sur Udemy : [Automatiser tout sur vos projets avec Github Actions](https://www.udemy.com/course/automatiser-tout-sur-vos-projets-avec-github-actions/?referralCode=268A353A1CAE10611EBD).

N'hésitez pas à explorer les fonctionnalités de Chromatic et de Storybook pour améliorer la qualité et la robustesse de vos composants d'interface utilisateur. Happy coding! 🚀
