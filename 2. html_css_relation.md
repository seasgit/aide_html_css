
# Introduction CSS
## Définition
CSS est l'acronyme de _Cascading Style Sheets_. 
Le terme _Cascade_ est en rapport avec des notions d'héritage et de surcharge de style. _(A voir en cours avec la pratique.)_  

Le langage CSS permet de mettre en page, d'aligner le contenu HTML, apporter un style répondant à une identité visuelle recherchée.   
Le lien HTML/CSS est à l'intérieur des balises `<head></head>` d'un document HTML.
```html
<head>
    <meta charset="UTF-8">
    <title>Titre du site</title>
    <link rel="stylesheet" href="style1.css">
    <link rel="stylesheet" href="style2.css">
</head>
```
Un document html peut aussi contenir du style css de la manière suivante:
```html
<head>
    <meta charset="UTF-8">
    <title>Titre du site</title>
    <link rel="stylesheet" href="style1.css">
    <style>
        /* règles de style ici */
    </style>
</head>
``` 

## Règle de style
Si nous voulons donner un style à un titre par exemple, nous devons créer une règle css composée : 
* d'un sélecteur. Il fait le lien avec l'élément html
* d'une suite de propriétés placées entre __{ }__ et séparées chacune par un point virgule.
```css
h1{
    color: #FCC;
    font-weight:normal;
    letter-spacing :3px;
}
```
* Coder un texte de couleur verte de taille 40px avec une bordure, etc..."   



## L'inpecteur du navigateur
Il permet à l’intégrateur web de tester des balises html ou des règles css sans modifier sur le fichier source.   
Faites un clic droit sur la page et sélectionner. __Inspecteur__.

