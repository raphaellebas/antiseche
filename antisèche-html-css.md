# L'antisèche

Ce guide à pour but de faire une cure de rappel pour les poissons rouge sur le langage [HTML](https://fr.wikipedia.org/wiki/Hypertext_Markup_Language), [CSS](https://fr.wikipedia.org/wiki/Feuilles_de_style_en_cascade) vu pendant mon parcours d'apprentissage ou professionnel.

- ## Sommaire

  - [L'introduction au HTML](#html-cest-quoi-)
  - [L'introduction au CSS](#css-cest-quoi-)

# HTML c'est quoi ?

  HTML est un langage très simple crée en 1991 par [Tim Berners-Lee](https://fr.wikipedia.org/wiki/Tim_Berners-Lee) et aider par l'ingénieur [Robert Cailliau](https://fr.wikipedia.org/wiki/Robert_Cailliau)ce langage est composé **d'éléments appliquables** à des **fragments** de texte dans un document pour leur donner un sens différent (Est-ce un paragraphe, est-ce une liste ? est-ce une puce ? ou est-ce une partie de tableau ?),
  pour structurer un document en section logiques (a-t'il un en-tête ? est-il sur trois colonnes ? a-t'il un menu de navigation ?)

## Le corps d'une page HTML

  Voyons ça comme un corps humain : 

   '|' -> Head (La tête)</br>
   /|\ -> Body (Le corps)</br>
   / \

   Dans un document **head**(La tête) c'est la partie du document qui n'est pas affiché par le navigateur au chargement de la page, elle contient des informations comme par exemple le titre ```<title>```
   de la page des liens **CSS** (La feuille de style) des liens pour le favicon (L'icon de la page qui apparaît dans les onglets) et des méta-données (Auteur du documents des mots clés qui décrit le documents etc..) L'HTML est composé généralement de Tag (Balise en Français) ouvrantes et tag fermantes

   exemple :

   ```<p>Mon Chat fait meow</p>```
   On peut voir que nous ouvrons la balise ```<p>``` qui est une balaise paragraphe "Mon chat fait meow" est le contenu et le ```</p>``` est la balise fermante.

## Wireframe 
  Le Wireframe un est shéma simple d'un site pas d'image pas de couleur, si vous voulez representer une image il suffit de faire une croix dans un rectangle ou cercle celà dépend la forme de l'image

## Création d'un formulaire
  
  Grâce à la balise ```<form>``` nous pouvons créer des formulaires 

  Le formulaire est composé de balise ```<label>``` et de balise ```input ```
 exemple :
  ```HTML
      <div>
            <form>
      
                <label for="lastname">Nom</label>
                <input type="text" id="lastname" name="lastname"  pattern="[a-zA-ZÀ-ÿ]{3,25}" title="Veuillez mettre au moins 3 caractères ou plus seulement les lettres sont                       autorisées" placeholder="Nom"  required>
      
             </form>
        </div>
  ```
> <input type="text" -> Le type de l'input est de type on lui donne l'id "lastname" on lui donne ensuite un pattern qui va prendre une expression régulière dans cette expression on dit qu'on autorise l'utilisateur à mettre des lettres en minuscules majuscules ou des accent on lui donne aussi un minimum de lettre à rentré donc 3 et un maximum donc 25 le title est une erreur qu'on va afficher au cas où il ne respect pas les conditions le placeholder (Espace reservé)  c'est un texte par défault qui est dans le champ.

## class
 
 L'atribut universel class indique une liste de classes associées à l'élément courant. Les classes permettent de manipuler les éléments via CSS ou JavaScript en utilisant les sélecteur de classe ou de fonctions telles que document.getElementsByClassName

 ## Comment créer une class en HTML?

```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mon expérimentation CSS</title>
    <link rel="stylesheet" href="/assets/css/style.css"> 
  </head>
  <body>
    <h1>Hello World!</h1>
    <p class="expérimentation">Ceci est mon expérimentation du CSS</p> <!--On attribut à la balise P la class "expérimentation"--> 
  </body>
</html>
```

## id

L'atribut universel id définit un identifiant qui doit être **unique** pour l'ensemble du document. Le but de cet attribut est de pouvoir identifier un élément lorsqu'on crée un lien avec un **fragment** et qu'on souhaite le manipuler avec un script ou qu'on le met en forme CSS.

```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mon expérimentation CSS</title>
    <link rel="stylesheet" href="/assets/css/style.css"> 
  </head>
  <body>
    <h1>Hello World!</h1>
    <p id="expérimentation">Ceci est mon expérimentation du CSS</p> <!--On attribut à la balise P la l'id "expérimentation"--> 
  </body>
</html>
```

# CSS C'est quoi ?

  ## Le CSS : Feuilles de style
  
  Le CSS est un des langages de la saint trinité du web ouvert, il a été standarisé par <a href="https://w3.org/Style/CSS/#specs">W3C</a>

    Ce standard évolue sous 3 levels

    Level 1 CSS1 est complètement obsolète

    Level 2 CSS2 correspond à la recommandation 

    Level 3 CSS3 il est découpé en modules plus petits, il est également en voie de standarisation.

  ## C'est quoi les bases du CSS ?

  Pour le bon fonctionnement le CSS possède des **unités** : 
  
  - Des Sélecteurs
  - Des Propriétés
  - On peut également écrire des règles
  - Appliquer du CSS dans un document **HTML**
  - Utiliser des longeurs
  - Mettre des couleurs et encore pleins d'autres **unités**.

  ## Nous pouvons également toucher au texte
  
  - Changer la police 
  - Mettre en gras
  - Mettre en italique
  - Gérer les espaces entre les lignes et les lettres
  - Ajouter des ombres portées etc.

## Mettre en forme les boîtes en (en-US)

  La mise en forme des boîtes en CSS sont un composant **clé** de la mise en page d'une page web.

## Les  Concepteurs majeurs du CSS

  - La syntaxe et les formes du langage 
  - La spécifité et l'héritage
  - Les unités et les valeurs CSS
  - Le modèle de boîte et la fusion des marges (en-US)
  - Le bloc conteneurs (en-US)
  - L'empilement et le contexte de formatage de blocs
  - Les concepts de valeur initiale, valeur calculée, valeur utilisées et valeur réelle
  - Les propriétés raccourcies
  - Les boîtes de flexibles CSS (flexbox)
  - La grille CSS
  - Les médias queries (requêtes media)
  - Les animations

## Le livres des recettes 

  Le livre de recettes de disposition CSS contient différentes recettes pour mettre en place différentes dispositions courantes.


## Comment ça fonctionne ?

```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mon expérimentation CSS</title>
    <link rel="stylesheet" href="/assets/css/style.css"> <!--<- Ici on fait appel au fichier style.css qui se trouve dans /assets/css/-->
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>Ceci est mon expérimentation du CSS</p> 
  </body>
</html>
```
Résultat :

<img src="https://github.com/raphaellebas/antiseche/blob/master/images/withoutcss.png?raw=true" alt ="Image représentant du HTML sans CSS">

Dans notre exemple on veut lui donner une couleur, une taille ainsi qu'une police d'écriture Times New Roman', Times, serif
> ATTENTION Si vous ajoutez ça à la balise ```<p>``` une couleur une taille ainsi qu'une police d'écriture TOUTES les balises ```<p>``` seront touchés.

# Côté CSS

```CSS
p{
    color: red;
    font-size: 16px;
    font-family: 'Times New Roman', Times, serif;
}
```

Résultat :

<img src="https://github.com/raphaellebas/antiseche/blob/master/images/withcss.png?raw=true" alt="image représentant l'exemple avec CSS">

## Ajouter du CSS avec une class 

  Comme dans le cours plus haut sur les classes nous pouvons faire appelle à une class dans le CSS 

  ```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mon expérimentation CSS</title>
    <link rel="stylesheet" href="/assets/css/style.css">
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>Ceci est mon expérimentation sans class</p>
    <p class="expérimentation">Ceci est mon expérimentation du CSS avec une class</p> 
    <p class="expérimentation2">Ceci est mon expérimentation du CSS avec une class</p> 
  </body>
</html>
```

On veut donner à notre class la couleur rouge et une taille de 32 px à la class expérimentation et la couleur bleue et la taille 5px à expérimentation2
> Pour faire appelle à une classe dans du css on commence par un point et ensuite le nom de la class

## Côté CSS

```css
.expérimentation{
  color:red;
  font-size:32px;
}

.expérimentation2{
  color:blue;
  font-size:5px;
}

```

Résultat :

<img src="https://github.com/raphaellebas/antiseche/blob/master/images/withclass.png?raw=true" alt="Image représentant deux balises avec deux classes différentes"> 

Cette fois-ci on veut utiliser l'id mais on va aussi ajouter une class pour l'id expérimentation on va lui donner la couleur bleue avec une taille de 16px pour l'id expérimentation2 on va lui donner une couleur dégradé avec une taille de 32px et pour notre class on va lui donner donner une couleur jaune avec une taille de 64 et on va aussi également lui mettre une propriété qui va nous permettre de changer de couleur qunad on passe le curseur dessus

  ```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mon expérimentation CSS</title>
    <link rel="stylesheet" href="/assets/css/style.css">
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>Ceci est mon expérimentation sans class</p>
    <p id="expérimentation">Ceci est mon expérimentation du CSS avec un id</p> 
    <p id="expérimentation2">Ceci est mon expérimentation du CSS avec un id</p>
    <p class="expérimentation3">Ceci est mon exéirimentation du CSS avec une class</p> 
  </body>
</html>
```
>Pour faire appelle à un id dans un css on mets un # avant le nom

## Côté CSS

```CSS
#experimentation{
    color:blue;
    font-size:16px;
}

#experimentation2{
    background: linear-gradient(90deg, rgb(252, 0, 105) 0%, rgb(0, 119, 255) 35%, rgba(0,212,255,1) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size:32px;
}

.experimentation3{
    font-size: 64px;
    color: rgb(252, 0, 105);
}


.experimentation3:hover{
    color: rgb(0, 119, 255);
}
```
