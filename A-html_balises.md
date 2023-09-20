
# 1. HTML5
## définition
HTML est l'acronyme de `HyperText Markup Langage`.   
HTML est un langage de balisage dont le rôle est de structurer le contenu de pages web. 
La version avec laquelle nous travaillons est HTML5.  
On parle de __HTML5 sémantique__ car ses balises ont un rôle plus précis qu'avant dans la gestion du contenu d'un site web.
## Ressources en ligne
Comme indiqué dans la pahe Home, La documentation proposée par Mozilla est exhausitive.   
On peut trouver aussi des résultats à partir d'un recherche par mots clé. On tape par exemple dans google _"html élément titre"_   

# 2. Structure d'un document HTML

## Visual Studio Code

Toujours faire `ouvrir un dossier` ou `nouveau dossier` afin d'avoir l'onglet gauche des dossiers et fichiers.  

![](./captures/open-folder.jpg)

Créer un Fichier avec un nom sans accent ni espace : __first-page.html__  
Une fois créé, le code ci-dessous peut être produit en tapant __!__ puis touche __tab__ ou __entrée__, selon l'IDE.
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Document</title>
    </head>
    <body>
        <!-- contenu de la page -->
    </body>
</html>
```
## Dans `<head>`
La balise head ne s'affiche pas dans le document, elle contient tout ce dont à besoin la page pour s'afficher et fonctionner correctement.    _styles, scripts, polices de caractères, et autres metadonnées_. 
## Dans `<body>`
C'est là qu'on intègre le contenu de la page dans des balises qui représenteront le mieux chaque élément de la page.  
* Un titre de page : `<h1>Carnet de route</h1>`
* Un article de blog :  `<article> <!-- contenu --> </article>`  


# 3. Les balises de contenu textuel et image
 

## Titres `<h1>-<h6> `
Documentation : [headings elements](https://developer.mozilla.org/fr/docs/Web/HTML/Element/Heading_Elements)  
Reproduire dans visual studio code, dans le body.
```html
    <body>
        <!-- contenu de page -->
    </body>
```
Puis `Faire un clic droit dans la page`  

![](./captures/open-live.jpg)


## Paragraphes `<p>`
Documentation : [headings elements](https://developer.mozilla.org/fr/docs/Web/HTML/Element/p)
## Balise `<span>`
Très utile pour mettre en évidence un ou plusieurs mots dans un bloc de texte paragraphe par exemple.
Le span prend toute son importance avec le style css.  
documentation [span](https://developer.mozilla.org/fr/docs/Web/HTML/Element/span)
## Listes `<ul> ou <ol>`
Documentation : [Listes](https://developer.mozilla.org/fr/docs/Web/HTML/Element/ul)
# 4. balises de séparation
## Saut de ligne `<br>` 
C'est une balise isolée qui permet un saut de ligne.    
documentation [br](https://developer.mozilla.org/fr/docs/Web/HTML/Element/br)    
## Trait horizontal `<hr>` 
documentation [hr](https://developer.mozilla.org/fr/docs/Web/HTML/Element/hr) 

## Images `<img>`
Documentation : [Images](https://developer.mozilla.org/fr/docs/Web/HTML/Element/Img)


# 5. Liens vers des fichiers externes
## Adressage relatif ou absolu
Les liens vers des fichiers externes peuvent être fait de 2 manières.  
## Adressage absolu
On donne l'url complète du document.  
    - Source d'une image :  
    `<img src='https://images.pexels.com/photos/2775862/pexels-photo-2775862.jpeg' />`
    - Lien vers Google :   
    `<a href="https://www.google.com" target="_blank">Page d'accueil Google</a>`    
## Adressage relatif 
On donne une adresse qui est relative à l'emplacement du fichier appelant au sein d'une architecture de dossiers d'un site web.
    - Ici une image placée dans le même que le document appelant :  
    `<img src='./pexels-photo-2775862.jpeg' />`     
    - Ici une image contenue dans un sous-dossier nommé _images_ :  
    `<img src='./images/pexels-photo-2775862.jpeg' />`  
    - Là une image contenue dans un dossier nommé _images_ en amont du fichier appelant :  
    `<img src='../images/pexels-photo-2775862.jpeg' />`  
## Lien hypertexte `<a>` 
documentation [Ancres](https://developer.mozilla.org/fr/docs/Web/HTML/Element/a)  
L'url peut être  : 
- absolue `<a href="https://example.com">Website</a>`
- relative. Le fichier requis doit être dans le dossier projet `<a href="./contact.html">contact</a>`



# 6. Les balises conteneur
Les conteneurs permettent de regrouper plusieurs contenus dans des balises sémantiques.
Le balises dites conteneur, prennetnt toute leur importance avec css dans la construction de modèles de pages web. 
## `<div>`
C'est le plus ancien conteneur. Il n'est pas sémantique. [div](https://developer.mozilla.org/fr/docs/Web/HTML/Element/div) 
## `<article>`
Par exemple pour un blog. [article](https://developer.mozilla.org/fr/docs/Web/HTML/Element/article) 
## `<figure>`
Par exemple pour un blog. [figure](https://developer.mozilla.org/fr/docs/Web/HTML/Element/figure) 
## A retenir
Selon le cas, on peut trouver une balise nommée `<article>`, ou encore `<figure>`.

Il n'y a pas d'obligation à utiliser telle ou telle balise. C'est juste du bon sens et faciliter la lecture par les robots référenceurs.

documentation [structurer un document](https://developer.mozilla.org/fr/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure).  

