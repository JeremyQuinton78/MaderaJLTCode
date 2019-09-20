# Comment utiliser Git
## En étant sur master, récupérer d'abord la dernière version de master

`git pull origin master`

## Créer une branche (par feature, par dev, c'est comme vous voulez)

`git checkout -b nom_branche`

## Faire les modifs qu'on veut

## Une fois que les commits sont faits, si un autre contributeur a fait des modifications sur master

```
git checkout master
git pull origin master
git checkout nom_branche
git rebase master
```
## Résoudre les éventuels conflits

```
git checkout master
git merge nom_branche
git push origin master
```

## Supprimer la branche de travail
`git branch -D nom_branche`
## Créer une nouvelle branche pour réaliser les nouvelles modifs
`git checkout -b nom_branche_suivante`
## etc ...
