## Welcome to GitHub Pages
You can use the [editor on GitHub](https://github.com/serorl/doctab/edit/master/README.md) to maintain and preview the content for your website in Markdown files. Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

## GIT
Configurer en global ou local le nom et l'email
```
git config --global user.name "son nom"
git config --global user.email "lemail@toto.com"
```
```
git init
git add _mesfichiers__
git commit -m "first commit"
```
Ajouter un dépot distant ` git clone https://distant  sous-repertoire-local`  depuis le répertoire parent.
**Attention** : Après le clonage d'un repo distant en cas de modification en local, ne pas oublier d'ajouter tous les fichiers `git add fichiers` utiles puis ` commit -m "message` , avant de faire un git push ..

Mise à jour du dépot distant `git push -u master` ou utiliser `git pull` si le dépot distant est plus à jour.
La commande `git fetch --all` télécharge sans fusionner les documents. Permet de connaitre l'état comparatif.


Pour les dépots git hub, il est nécessaire d'utiliser le logiciel console GH 
` $> apt instal gh `
Les commandes sont différentes de git. `$> gh auth login` , pour ajouter l'appareil au repository.
[ documentation Git Hub Cli ](https://cli.github.com/manual/)


## Markdown
```markdown
Syntax highlighted code block
# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/serorl/doctab/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
