# L'antisèche

Ce guide à pour but de faire une cure de rappel pour les poissons rouge sur le langage [HTML](https://fr.wikipedia.org/wiki/Hypertext_Markup_Language), [CSS](https://fr.wikipedia.org/wiki/Feuilles_de_style_en_cascade) vu pendant mon parcours d'apprentissage ou professionnel.

- ## Sommaire

  - [L'introduction au HTML](#html-cest-quoi-)


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
