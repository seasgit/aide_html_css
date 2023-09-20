
# 1. Quelques unités dans les propriétés css
|Unités| infos |
|:---:|:---|
| px | Taille absolue exprimée en pixel. |
| % | Pourcentage de largeur ou hauteur de l'élément parent. Utilisé avec les largeurs de blocs, d'images |
| rem |	Unité relative à la taille par défaut du corps.|
| vw / vh |	Unité relative à l’écran. (v comme viewport) |

# 2. Unités en pixel
### Exemple codepen [unites](https://codepen.io/seasgit/pen/dyeNNMp)


Testez avec l'inspecteur. Changer la font-size du body, et constatez ! ... Aucun changement !  
De plus, si je décide que le paragraphe a une taille de 18 pixel, je dois recalculer la taille de son span pour qu'il reste à 140%.  
Pas très pratique !
# 3. Unité relative __rem__
Unité adaptée à des agrandissements simple d'utilisation.  
La proportionalité se fait à partir de la taille par défaut du navigateur.

### Exemple codepen [unites](https://codepen.io/seasgit/pen/wvjggmY)

Utiliser aussi ce site pour faire quelques conversions : https://www.jarrige.fr/pixelrem/

# 4. Un mot sur les unités viewport
Ce système d'unité est plus récent. Les valeurs sont relatives à la largeur ou la hauteur de l'écran.
- 10vh  =  10% de la hauteur du viewport.    
- 10vw  =  10% de la largeur du viewport.    
- 10vmin = 10% de la dimension la plus petite de la fenêtre.  

__A noter__ qu'elles sont de plus en plus utilisées, d'autant plus avec les besoins liés au reponsive web design. 

