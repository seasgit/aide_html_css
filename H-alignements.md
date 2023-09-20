
# Propriété display 
La propriété display permet de définir le type d'alignement d'élements dans une page ou dans une boîte.  
Il existe beaucoup de possibilités d'alignments.  
###
[display](https://developer.mozilla.org/fr/docs/Web/CSS/display)

## display:block versus display:inline
Un élément tel que le _div_ a par défaut la propriété `display:block`.  
Un élément tel que le _span_ a par défaut la propriété `display:inline`.  
On peut voir dans l'exemple suivant le résultat.  
  (_Enlevez dans un 2ème temps les commentaires et constatez le changement._)
  
  [display block vs inline](https://codepen.io/seasgit/pen/mdLMoOZ)

## display: none vs visiblity: hidden
Quand on veut masquer un élément de la page il y a deux possibilités : 
Avec `display:none` la place est récupérée par le navigateur. Cela peut créer un décalage.    
Dans certains cas il vaudra mieux utiliser `visibility: hidden`.  

[Exemple](https://codepen.io/seasgit/pen/wvjqOeM)


# Flexbox  ou "_CSS Flexible Box Layout Module_". 
Flexbox permet d'aligner intelligemment des éléments de page dans des conteneurs.  

> __A retenir :__  
	Un conteneur de type flex aligne ses enfants __directs__.  
	Un élément enfant d’un conteneur flex peut gérer son propre alignement.  

## quelques bases
Dans l'exemple ci-dessous, nous voyons comment 3 boites s'alignent horizontalement dans un conteneur.  

[Simple alignement de boîtes](https://codepen.io/seasgit/pen/XWqaGqY)

Dans l'exemple ci-dessous, nous voyons comment répartir horizontalement les boîtes.  
Plusieurs possibilités à tester.  

[Répartir horizontalement les boîtes](https://codepen.io/seasgit/pen/PoeKLXN)

Dans l'exemple ci-dessous nous voyons comment aligner verticalement.  
__A noter__ que le conteneur doit avoir une hauteur.

[Aligner verticalement](https://codepen.io/seasgit/pen/oNdeVVr)

## Ressources   
https://css-tricks.com/snippets/css/a-guide-to-flexbox/    
https://codepen.io/enxaneta/full/adLPwv/  

## Tutoriels
https://www.youtube.com/watch?v=Y8zMYaD1bz0&list=PL4cUxeGkcC9i3FXJSUfmsNOx8E7u6UuhG  

## Jeux
http://flexboxfroggy.com/    
http://www.flexboxdefense.com/  

