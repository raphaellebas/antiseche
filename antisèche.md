# L'antisèche

Ce guide à pour but de faire une cure de rappel pour les poissons rouge sur les commandes [Linux](https://www.linux.org), [Git](https://git-scm.com) et sur d'autres thème vu pendant mon parcours d'apprentissage ou professionnel.

- ## Somaire

  - [Qu'est-ce que c'est Linux ?](#linux)
  - [Pourquoi utiliser le Terminal ?](#pourquoi-utiliser-le-terminal-)
  - [Les différentes commandes apprises](#les-différentes-commandes-apprises)
  - [C'est quoi Git?](#git)
  - [Pourquoi utiliser git ?](pourquoi-utiliser-git-)
  - [Les différentes commandes apprises](#les-différentes-commandes-apprises)

# Linux
  
  Linux est une famille de système d'exploitation **open source** gratuit de type **Unix-like** fondé en 1991 par son papa [Linus Torvalds](https://fr.wikipedia.org/wiki/Linus_Torvalds) il a vu au jour une centaine de distributions.
 
 ### Les Principales distributions :
   - [Debian](https://www.debian.org/index.fr.html)
   - [Redhat](https://www.redhat.com/fr)
   - [Archlinux](https://archlinux.org)
   - [Android](https://www.android.com/intl/fr_fr/)

- ## Pourquoi utiliser le terminal ?
     L'utilité du Terminal facilite la vie des devs, il permet ainsi être plus pointieux sur des commandes qu'on ne pourrait pas forcément lancer en interface graphique.
     Il rend aussi également plus rapide le lancement des programmes vu qu'il ne possède pas d'interface graphique.
     
## Les différentes commandes apprises

> Ps : Ceci est les différentes commandes que j'ai pu apprendre durant mon pourcours d'apprentissage ou professionnel.

### Les commandes simples MAIS utile !

```ls```
Cette commande permet de lister le contenu d'un dossier.

Resultat :
``` 
    lua@DESKTOP-QECQM4H  ~  ls                                                                    
    antisèche  git_workspace  powerlevel10k  test 
```

> Il se peut que vous avez des fichiers invisible alors ajouter un -a après ls ça listera tout les fichiers y compris ceux qu'on ne voit pas.
    
```cd chemin/chemin```
Cette commande permet de changer de dossier (en gros se déplacer dans les dossiers).

Résultat :
```
 lua@DESKTOP-QECQM4H  ~  pwd                                                                   
   /home/lua
 lua@DESKTOP-QECQM4H  ~  cd antisèche                                                          
 lua@DESKTOP-QECQM4H  ~/antisèche  master 
```

```pwd```
Cette commande permet d'afficher le chemin du dossier dans lequel on se trouve.

Résultat : 
```
lua@DESKTOP-QECQM4H  ~  pwd                                                                   
  /home/lua
```

```cat```
Cette commande permet d'afficher et de concaténer le contenu de fichiers.

> Si vous connaissez déjà le chemin de votre fichier vous pouvez faire directement un ```cat ~/chemin/fichier ``` .

Résultat :
```
 lua@DESKTOP-QECQM4H  ~  cat newfile.txt                                                       
  Bonjour tout le monde je suis un fichier txt :)
```

```clear```
Cette commande permet de nettoyer le terminal.

Résultat :

[![https://github.com/raphaellebas/antiseche/blob/master/images/clear.gif](./images/clear.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/clear.gif)

```ctrl-c```
Ce raccourci clavier permet de tuer le processus en cours.

Résultat :

[![https://github.com/raphaellebas/antiseche/blob/master/images/ctrl-c.gif](./images/ctrl-c.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/ctrl-c.gif)

```exit```
Cette commande permet de quitter le shell ou une session en cours.

Résultat :

```
bandit0@bandit:~$ exit
  logout
  Connection to bandit.labs.overthewire.org closed.
lua@DESKTOP-QECQM4H  ~ 
```

```man```
Cette commande permet d'afficher le manuel.

```mkdir nomdudossier```
Cette commande permet de créer un dossier.

Résultat :

```
 lua@DESKTOP-QECQM4H  ~  ls                                                                    
  antisèche  git_workspace  newfile.html  powerlevel10k  test
 lua@DESKTOP-QECQM4H  ~  mkdir nouveaudossier                                                  
 lua@DESKTOP-QECQM4H  ~  ls                                                                    
  antisèche  git_workspace  newfile.html  nouveaudossier  powerlevel10k  test
 lua@DESKTOP-QECQM4H  ~ 

```

```nano```
Cette commande permet d'ouvrir l'éditeur de texte intégré dans le terminal.

Résultat : 

[![https://github.com/raphaellebas/antiseche/blob/master/images/nano.gif](./images/nano.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/nano.gif)

> Vous pouvez créer un nouveau fichier en faisant juste ```nano newfile``` suivit de son extension de fichier exemple : ```.txt,.html,.css, etc...```.

```rmdir nomdudossier```
Cette commande permet de supprimer un dossier.

Résultat : 

[![https://github.com/raphaellebas/antiseche/blob/master/images/rmdir.gif](./images/rmdir.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/rmdir.gif)

> Si vous avez créer des dossiers dans le dossiers parent et que vous voulez le supprimer faites ```rmdir nomdudossierparent/dossierquejesouhaitesupprimer ``` il supprimera alors le dossier enfant visé.

```rm -v nomduchemin/nomduchemin```
Cette commmande permet de supprimer tout les fichiers d'un chemin.

Résultat :

[![https://github.com/raphaellebas/antiseche/blob/master/images/removeallfiles.png](./images/removeallfiles.png)](https://github.com/raphaellebas/antiseche/blob/master/images/removeallfiles.png)

```touch nomdufichier.extension```
Cette commande permet de créer un fichier

Résultat : 

[![https://github.com/raphaellebas/antiseche/blob/master/images/touch.gif](./images/touch.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/touch.gif)

> Vous pouvez créer plusieurs fichiers en une seul commande ```touch readme.md,index.html,.style.css,script.jss``` il suffit juste de séparé les fichiers avec une virgule.

```mv nomdufichier chemin/```
Cette commande permet de déplacer un fichier dans un autre chemin

Résultat : 

[![https://github.com/raphaellebas/antiseche/blob/master/images/move.gif](./images/move.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/move.gif)

> Vous pouvez déplacer le fichier au dossier parent il suffit juste d'ajouter ```../``` à la place d'un nom de dossier

```mv oldname newname```
Cette commande permet de rename un fichier

Résultat :

[![https://github.com/raphaellebas/antiseche/blob/master/images/rename.gif](./images/rename.gif)](https://github.com/raphaellebas/antiseche/blob/master/images/rename.gif)

> Vous pouvez rendre un fichier ou un dossier invisible juste avec un point au début du nom de celui-ci, il ne s'affichera pas en faisant ```ls``` .
> Pour celà ```mv nomdufichieroudossier .nomdufichieroudosier``` 

```find```
Cette commande permet de chercher un fichier dans un répertoire.

Résultat : 

```
lua@DESKTOP-QECQM4H  ~/antisèche/images  master  ls                                        
  clear.gif  ctrl-c.gif  move.gif  nano.gif  removeallfiles.png  rename.gif  rmdir.gif  terminal.png  touch.gif
lua@DESKTOP-QECQM4H  ~/antisèche/images master  cd ../../                                 
lua@DESKTOP-QECQM4H  ~  find ./antisèche -name clear.gif                                      
  ./antisèche/images/clear.gif
```

```ssh```

Cette commande ```ssh``` (**Secure Shell**) permet de se **connecté** à un **server** en toute **sécurité**.

Résultat :

```
  ssh bandit0@bandit.labs.overthewire.org -p 2220
```

> ssh --> La commande Secure Shell bandit0--> le nom d'utilisateur bandit.labs.overthewire.org--> l'host -p--> le port 2220--> le numéro de port




# Git
  
  Git est un système de contrôle de vesion open source. Sa première version a vu le jour en 2005, conçu par le même créateur de Linux [Linus Torvalds](https://fr.wikipedia.org/wiki/Linus_Torvalds).
  Grâce à Git les devs peuvent héberger leur code appellées forges tels que [Github](https://github.com), [Gitlab](https://gitlab.com/gitlab-org) ou encore [Bitbucket](https://bitbucket.org).

- ## Pourquoi utiliser git ?
    Git est un outil primordial dans le monde du développement, il permet de facilité le travail en équipe ainsi que créer des back-up.

## Les différentes commandes apprises