# 1. Introduction  
Une boîte possède des dimensions et peut apparaître sur la page comme une forme rectangulaire.    
Un simple paragraphe peut être vu comme une « boîte ».  
En pratique on relie souvent le terme boite à un conteneur.  
# 2. Caractéristiques d'une boîte  :
* Elément de type block.   `display:block`
* possède une largeur et hauteur.   `width|height`
* peut avoir un espace interne tout autour.   `padding`
* peut avoir des marges externes.   `margin`
* peut avoir des bordures.   `border`
## 
> __Démo :__ http://guyroutledge.github.io/box-model/ 
##
> __Mozilla doc__ : https://developer.mozilla.org/fr/docs/Web/CSS/border

# 3. Ne sont pas des boîtes
les élements de type `inline`, comme :
* les hyperliens, appelées aussi ancres. `<a>` 
* les images. `<img />`
* les éléments relatifs aux paragraphes : `<span>, <em>, <strong>, ...` pour ne citer que ceux là. 

# 4. Exercices

### [Boîte simple](https://codepen.io/seasgit/pen/jOxVpYo)
## Bordures
### [Boîte avec bordures](https://codepen.io/seasgit/pen/xxjdjKw)
### [Boîte avec bordure haute](https://codepen.io/seasgit/pen/WNJjJba)
## marges
### [Boîte avec marges](https://codepen.io/seasgit/pen/bGMWMVj)
### [Boîte centrage avec marges](https://codepen.io/seasgit/pen/MWGmGyM)
## Espace interne
### [Boîte avec padding](https://codepen.io/seasgit/pen/ExLmLWK)
Le padding d’une boîte se traduit par une dilatation de celle-ci.  
Le padding peut nuire à une mise en page s'il est appliqué sans réelle 
étude du gabarit de page.  

__A NOTER__   
CSS3 propose la propriété `box-sizing :border-box`.  
L’espace est recalculé afin de s’adapter au mieux aux dimensions d’origine du conteneur.


