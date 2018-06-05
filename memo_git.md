# Memo Git - GitHub #

### Configuration de git ###
**`git config --global user.email "you@example.com"`**  
**`git config --global user.name "Your Name"`**  

### Commande de base ###
**`git init`** :  Créer un nouveau repository (dossier git).  
**`git add mon_fichier`** : Ajoute un fichier présent dans le dossier au repository.  
**`git commit -m "Description précise"`** : Enregistre l’état du projet quand un fichier vient d’être enregistré.  
**`git commit -am "Description précise`** : Enregistre l'état du projet quand on a fait une modification sur un fichier existant.  
**`git log`** : Affiche le journal des commits (historique du projet).  
**`git checkout SHA_dun_commit`** : Nous place au commit sélectionné (retour en arrière en cas d'erreur par exemple).  
**`git checkout master`** : Nous positionne sur le dernier commit.  

**********************************************************************************************************************************
### Github (nécéssite un compte sur [github](https://github.com/)) ###
**`git clone URL`** : Clône en local un projet git.  
**`git push origin master`** : Envois les commits local sur github *(demande login et mdp)*.  
**`git pull origin master`** : Récupère les mises à jours depuis github.  

Dans le cas ou le projet serais déja existant et que vous vouler le mettre sur github : 
1. Créer un nouveau repository sur [github](https://github.com/) ayant le meme nom que le dossier dans lequel est le projet.
2. Faire un **`git init`** dans le dossier du projet.
3. Faire un **`git add *`**.
4. Puis un **`git commit -m "Description précise"`**.
5. Et enfin **`git remote add origin URL_du_projet_git`**, le liens entre votre dossier et github sera établit. Il ne restera plus qu'a faire un push.

**********************************************************************************************************************************
### Branche ###
**`git branch`** : Liste les branches du projet.  
**`git branch ma_branche`** : Créer une branche nommé *ma_branche*.  
**`git checkout ma_branche`** : Nous positionne sur la branche nommée.  
**`git checkout -b ma_branche`** : Créer une branche ma_branche et nous positionne dessus.  
**`git merge ma_branche`** : Fusionne la branche courante (sur laquelle on est) avec la branche nommée.  

En cas de conflit pendant un **merge** : Résoudre manuellement puis refaire un **add** et un **commit** du fichier impacté.  

**********************************************************************************************************************************
###  Ignorer un fichier ###
1. Créer un fichier **.gitignore** à la racine du projet.   
2. Lister les fichiers à ignorer (ex : fichier de configuration, ou tous fichier contenant des données sensibles).  
3. Faire un **`git add .gitignore`**.  
4. Puis un **`git commit -m "Description précise"`**.  

**********************************************************************************************************************************
### Divers ###
**`git blame mon_fichier`** : Affiche l'auteur ligne par ligne du fichier nommé.  
**`git show SHA_dun_commit`** : permet de voir ligne par ligne les modifications apporter par fichiers impactés pour le commit nommé.  
**`git stach`** : Met de coté le travail fait sans le commit *(pour modifier rapidement une autre branche en urgence par exemple)*.  
**`git stash pop`** : Récupère le travail mis de coté *(Détruit le stash = plus de sauvegarde du travail)*.  

Un Fork et une copie d'un projet public pour soit.  

****************************************************************************************************************
Résultat d'un tuto réalisé sur le site [openclassroom](https://openclassrooms.com/). Mis sous forme de mémo d’après ma compréhension du sujet. Je ne pourrais en aucuns cas être tenu responsable suite à une mauvaise utilisation ou une mauvaise compréhension de ce mémo.
Merais
