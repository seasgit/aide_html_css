
# 1. Un mot sur le flux normal 
Le flux normal est défini par la spécification CSS 2.1. Elle explique comment les boîtes du flux normal s'inscrivent dans le contexte de formatage.  
Les boîtes peuvent être de bloc (block) ou en ligne (inline) mais pas les deux à la fois. 
*  __block__ les éléments se placent les uns au dessous des autres.
*  __inline__ les éléments se placent à l'horizontale de gauche à droite.  

[source mozilla](https://developer.mozilla.org/fr/docs/Web/CSS/CSS_Flow_Layout/Disposition_de_bloc_en_ligne_avec_flux_normal)  

# 2. Position static
C’est la position par défaut d’un objet dans du flux normal.
# 3. Position relative
Un élément en position relative peut être déplacé en utilisant ses propriétés css __left__ et __top__.
## Exemple 1 : 
3 rectangles sont alignés les uns au dessous des autres. Grâce à la position relative, le 1er est décalé en diagonale. 
> Toutefois il reste dans le flux normal, ce qui peut provoquer un espace vide non désirable.  

[Exemple position relative](https://codepen.io/seasgit/pen/NWMgMdB)

## Exemple 2 :
Deux blocs utilisent la position relative pour intervertir leur position.  

[Exemple position relative](https://codepen.io/seasgit/pen/OJZgZmQ)

# 4. Position absolute
Un élement en position absolute est enlevé du flux normal. Sans autre indication, le  __body__ devient son parent direct.    
L’intérêt est aussi de pouvoir le placer n’importe en utilisant les prorpiétés __left, top, right, bottom__. 
## Exemple 1 : 
Une section rectangulaire contient un carré, lequel est en position absolute et ne s'affiche plus dans la section.      
Pour que le carré soit à nouveau relatif à son parent, le parent doit être en  __position relative__.

[Exemple position absolute](https://codepen.io/seasgit/pen/rNvwvGB)

## Exemple 2 :
Le code suivant crée la face 3 d'un dé à jouer.

[Exemple position absolute](https://codepen.io/seasgit/pen/OJZgZQZ)

# 5. Position fixed
Un élément fixe reste à sa place d’origine. L’exemple suivant montre  :
* comment fixer un menu. 
* comment fixer le background d’une section.

[Exemple position fixed](https://codepen.io/seasgit/pen/LYmLmrx)