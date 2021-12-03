# L'antisèche

Ce guide à pour but de faire une cure de rappel pour les poissons rouge sur les commandes du terminal [Linux](https://www.linux.org) et des commandes [Git](https://git-scm.com).

- ## Somaire

  - [Qu'est-ce que c'est Linux ?](#linux)
  - [Pourquoi utiliser le Terminal ?](#pourquoi-utiliser-le-terminal-)
  - [Les différentes commandes apprises](#les-différentes-commandes-apprises)
  - [C'est quoi Git?](#cest-quoi-git)
  - [Les différentes commandes apprises](#les-diff%e%rentes-commandes-apprises)

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
    lua@DESKTOP-QECQM4H  ~  ls                                                                     ✔  1043  23:39:45
    antisèche  git_workspace  powerlevel10k  test 
```
    
```cd```
Cette commande permet de changer de dossier (en gros se déplacer dans les dossiers).

Résultat :
```
 lua@DESKTOP-QECQM4H  ~  pwd                                                                    ✔  1044  23:39:47
   /home/lua
 lua@DESKTOP-QECQM4H  ~  cd antisèche                                                           ✔  1045  23:45:09
 lua@DESKTOP-QECQM4H  ~/antisèche   master 
```

```pwd```
Cette commande permet d'afficher le chemin du dossier dans lequel on se trouve.

Résultat : 
```
lua@DESKTOP-QECQM4H  ~  pwd                                                                    ✔  1044  23:39:47
  /home/lua
```

```cat```
Cette commande permet d'afficher et de concaténer le contenu de fichiers.

Résultat :
```
 lua@DESKTOP-QECQM4H  ~  cat newfile.txt                                                        ✔  1049  23:50:51
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
 lua@DESKTOP-QECQM4H  ~ 
```

```man```
Cette commande permet d'afficher le manuel.
