# 1. Introduction
Il existe plusieurs façons de relier un élement HTML à son style CSS. Tout passe par des __sélecteurs.__


Ce chapitre montre quelques manières. Les exercices permettront d'aller plus loin et comprendre l'intérêt de bien sélectionner 

# 2. Sélecteurs naturels
Les sélecteurs naturels font directement référence à des éléments html sans nom.  
## 
### [Exemple simple](https://codepen.io/seasgit/pen/abGpJJL)
## 
### [Exemple avec l'opérateur >](https://codepen.io/seasgit/pen/WNJRpKr)

##
__Attention__ : Sans maîtrise des sélecteurs naturels, on peut vite faire preuve d'imprécision voire de sélection globale.

# 3. Sélecteur par classes (.nom_classe)
Les sélecteurs classe, permettent de créer des catégories de règles css applicables à plusieurs éléments de même nature, ou ayant des rôles similaires.    
## 
### [Exemple avec classe simple](https://codepen.io/seasgit/pen/YzLNVpK)
## 
### [Exemple avec classes multiples](https://codepen.io/seasgit/pen/wvjgdoo)

# 4. Sélection par id
Un élément html identifié doit être unique dans une page. 
### [Exemple avec sélecteur id](https://codepen.io/seasgit/pen/WNJRjdZ)
## 

## Navigation interne  
Donner un attribut id sert aussi quand on doit naviguer au sein d’une même page.     
Pour cela il faut une correspondance entre le contenu d'un attribut href et celui d'un attribut id. 

### [Exemple](https://codepen.io/seasgit/pen/RwyKVJa)
## 


# 5. Pseudo classes
les pseudos classes sont des fonctionnalités associées au sélecteurs. On peut par exemple : 
-  gérer un survol sur un texte ou une boîte
-  cibler un élément via un numéro de positionnent
- 
## Effet de survol
Au survol de la souris sur un élement sa couleur change 
### [Exemple avec des ancres](https://codepen.io/seasgit/pen/xxjdYzJ)
### [Exemple avec un paragraphe et son span](https://codepen.io/seasgit/pen/WNJjMmR)

## Cibler un ou plusieurs éléments
Dans cet exemple, nous sélectionnons le 2ème élément de la liste et changeons sa couleur
### [élément précis d'une liste](https://codepen.io/seasgit/pen/zYjwWOJ)

### Voir aussi
    https://css-tricks.com/examples/nth-child-tester/
    http://nthmaster.com/  


# 6. Sélecteur :root
Utile par exemple pour créer des variables afin d'enregistrer des valeurs récurrentes d'une page web.
- Exp : couleurs, ombres, bordures, etc ...
Ci-dessous, une variable contient une couleur, l'autre les valeurs pour une ombre diffuse.
```css
:root {
  --color-primary: #eb2f64;
  --shadow-dark: 0 32px 96px rgba(0, 0, 0, .3); }
```
__NB__  :  une variable est appelée ensuite comme ceci : 
```css
.unebox {
  background-color: var(--color-primary);
}
```

# 7. Le poids des sélecteurs
IL est possible de perdre un peu avec les sélecteurs si nous ne maîtrisons pas l'ordre d'importance ou les combinaisons
des différents types de sélecteurs.  
Voyons cela avec un exemple pratique avec faire sous VSC ou codepen 
##  exemple 
Soit un paragraphe avec deux attributs : identifiant et class.
```html
<p class="p1" id="p1">HTML5 CSS</p>
```

```css
  /*  couleur donnée dans une règle avec sélecteur naturel */
p{
  font-size: 2rem;
  color :darkcyan
}
```
Puis, on attribue une couleur dans une règle avec un sélecteur de classe.
On constate que le texte devient vert.

```css
.p1 { color: green; }
```
On continue et ici on voit qu'avec le sélecteur identifiant, la couleur passe en orange
```css
#p1 {  color:orange }
```
Ajouter maintenant le style en ligne et constater !
```html
<p class="p1" id="p1" style='color:red'>HTML5 CSS</p>
```
Enfin, modifier le sélecteur naturel comme ceci :
```css
p{
  font-size: 32px!important;
  color :darkcyan
}
```
