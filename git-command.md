Configuration GIT

git config --global 
git config --global user.name "?"
git config --global user.mail "?"
git config --global core.editor "?"                                    Pour définir l'éditeur qui sera utiliser
git config --global --unset user.name "borelsaffo328@gmail.com"


git config --global  user.name          me retourne le username configurer
git config --global  user.email         me retourne l'émail configurer
git config --global  --list             me retorne tous les paramètre ou les variables déja défini ou déja configurer

git branch --list
git help config 
git add -h  

git log : 
git log -p -2 :         affiche les log avec les deux dernier commit
git log --graph : 
git log --prety-online : 
git config --global init.defaultBranch <nom> : 
git config --global init.defaultBranch master : 
git config --global init.defaultBranch dev : 



git rm   nom-du-fichier     : permet de ne plus tracker un fichier


GIT  Fonctionnement

Working Directory  :  c est mon repertoire de developpement, de travaill

Staging Area :   c'est l'environnement dans lequel on place tous les fichier modifier. lorsqu modifie un fichier qui se trouve dans le staging area 
                  et ensuite on effectue git add . le fichier modifier passe du working Directory au staging area.

Repository ou Directory : c'est le point central ou la version finale du fichier préalablement modifier est stocké a la suite d'un git commit


Git init : initialise le repository et viens aussi créer le dossier caché .git ce dossier contient un ensemble d'éléments permettant de géré le repos et 
           de tracker toutes les mdifications.


           etat des fichier avec Git: 
  Untracked : non suivi    nécessité d un  git add
  Unmodiified :  non modifier mais suivi
  Modified : modifier 
  staged : placer dans l'environnement de staging


  le fichier .gitigore permet de cacher certains fichier et dossier, il permet aussi de ne pas tracker certains fichier : *.log  /credential  /passwd   /image
           



Les tags
        git tag -a 1.0.0 -m "firt version of our apps"  :  permet de creer un tag 
        git tag -a 1.0.1 -m "second version of our apps" : 
        git tag :   affiche la liste des différent tag de l'application
        git show  1.0.0  :    affiche les détails sur ce tag (date de creation , auteur, les derniers commit avant sa realisation)

Les allias  
          config --global unset alias.br branch :                      équivalent a git br        retourne la branche courrante
          config --global unset alias.st status :                     équivalent a git st        retourne le status

Les branches git 
           git branch : ffiche la branche courrant de mon repository 
          git  checkout -b nom-de-la-nouvelle-branche-a-ceer : cette commande nous permet de se déplacer sur une nouvelle branche, 
                                                                     elle vas aussi creer cette branhe si elle n'existe pas encore
           git merge nom-de-la-branche-a-merger-avec la branche master : on le fait étant sur la branche master

Serveur Git
        

        git remote -v :  pour voir les différents depot distant
        git push origin nom-de-la-branche-a pousser :
