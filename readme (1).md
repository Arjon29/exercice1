# TP GIT

## Mise en place

* Installer Git si ça n'a pas déjà été fait
* Former des groupes de 2 ou 3

### Instructions

#### Dépôt Github

1. Création d'un dépôt sur Github par 1 personne du groupe
2. Toutes les personnes du groupe vont ensuite cloner le dépôt dans un dossier de votre serveur web (dossier www, htdocs...) à l'aide de la commande *git clone*
```
cd arborescence/vers/www
git clone https://github.com/{votre nom utilisateur}/{votre dépôt créé}.git
```

#### Création de fichiers et récupération

A tour de rôle :

* Une personne va créer un fichier {pseudo}.php
```php
<?php
	echo 'Hello world';
```
* L'ajouter à git (à l'aide de la commande git add -A)
* Faire le commit (git commit -m "votre message") et envoyer l'ajout vers github (git push -u origin main)

Les autres personnes : 
Récupérer les modifications apportées par la personne qui a créé le fichier
```
git pull origin main
```

#### Modifications sur le même fichier

Personne A :
* Une personne va créer un fichier *main.css* dans un dossier css
* L'ajouter à git
* Commit + push

Les autres personnes :
* Récupérer le fichier créé (git pull)
* Faire des modifications dans le fichier *main.css*
* Commit + push

Personne A :
* Faire des modifications dans le fichier *main.css* (ne pas récupérer le fichier avant)
* Commit + push
* Qu'est-ce que l'on constate ?