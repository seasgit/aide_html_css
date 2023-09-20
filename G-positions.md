
# Introduction
On aborde ici trois types de positions.  
__NB__ Attention, le positionnement est différent de l'alignement. Pour vous aider, associez position à _superposition_, _calque_
# Position relative
Un élément en position relative peut être déplacé en utilisant ses propriétés css __left__ et __top__.
## Exemple 1 : 
3 rectangles sont alignés les uns au dessous des autres. Grâce à la position relative, le 1er est décalé en diagonale. 
> Toutefois il reste dans le flux normal, ce qui peut provoquer un espace vide non désirable.  

[Exemple position relative](https://codepen.io/seasgit/pen/NWMgMdB)

## Exemple 2 :
Deux blocs utilisent la position relative pour intervertir leur position.  

[Exemple position relative](https://codepen.io/seasgit/pen/OJZgZmQ)

# Position absolute
Un élement en position absolute est enlevé du flux normal. Sans autre indication, le  __body__ devient son parent direct.    
L’intérêt est aussi de pouvoir le placer n’importe en utilisant les prorpiétés __left, top, right, bottom__. 
## Exemple 1 : 
Une section rectangulaire contient un carré, lequel est en position absolute et ne s'affiche plus dans la section.      
Pour que le carré soit à nouveau relatif à son parent, le parent doit être en  __position relative__.

[Exemple position absolute](https://codepen.io/seasgit/pen/rNvwvGB)

## Exemple 2 :
Le code suivant crée la face 3 d'un dé à jouer.

[Exemple position absolute](https://codepen.io/seasgit/pen/OJZgZQZ)

# Position fixed
Un élément fixe reste à sa place d’origine. L’exemple suivant montre  :
* comment fixer un menu. 
* comment fixer le background d’une section.

[Exemple position fixed](https://codepen.io/seasgit/pen/LYmLmrx)