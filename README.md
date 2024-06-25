# Crashlex
Solution unique pour les signets maladroits. Helpage vous permet d'organiser vos favoris personnalisés et vos sites les plus visités sur une page Web HTML5 de base.

***Crashlex*** est une page Web conçue dans le but de réduire le besoin d'onglet Favoris de tout navigateur classique. De plus, il contient des signets similaires à ceux d’un navigateur classique.

Helpage a été essayé et testé pendant des mois d'utilisation. Il a été témoin de centaines de ✅Changements, ⏫Mises à niveau, 📈Améliorations et 🐞 Corrections de bugs selon les besoins. C'est possible grâce aux efforts collaboratifs 🤝 de l'équipe.


# **Comment utiliser Helpage ?** *(Efficacement !!)*
Copiez l'URL https://crashlex08.github.io/Crashlex/
Accédez aux paramètres de votre navigateur.
Sous « Au démarrage » (ou toute option similaire), sélectionnez « Ouvrir une page ou un ensemble de pages spécifique ».
Ajoutez une nouvelle page et collez l'URL copiée.
Et vous êtes prêt à partir. 👍
Désormais, chaque fois que vous ouvrirez votre navigateur, vous aurez tous les sites Web sélectionnés au même endroit.
<br/><br/>

## Chrome :
![Chrome-Helpage](/images/helpageChrome.png)
## Brave:
![Brave-Helpage](/images/helpageBrave.png)
## Safari:
![Safari-Aide](/images/helpageSafari.png)


# 👷‍♂️**Comment personnaliser l'aide ?**

1. Forkez le référentiel.

2. Clonez le référentiel dans votre environnement local.

3. Une fois le référentiel cloné, vous devez l'ouvrir dans Git bash.

4. Créez une branche spécifique au problème sur lequel vous travaillez.
 ```coquille
 git checkout -b votre-nom-de-branche
 ```
 Pour plus de clarté, nommez
 votre branche `update-xxx` ou `fix-xxx`. Le « xxx » est une brève description des modifications que vous apportez. Les exemples incluent `update-readme` ou `fix-typo-on-contribution-md`.

5. Ouvrez le projet dans votre éditeur de texte préféré, sélectionnez le fichier auquel vous souhaitez contribuer et apportez vos modifications.

6. Ajoutez vos fichiers modifiés à Git.
 ```coquille
 git add chemin/vers/nom de fichier.ext
 ```
 Vous pouvez également ajouter tous les fichiers non préparés en utilisant :
 ```coquille
 git ajouter .
 ```

 **Remarque :** l'utilisation d'un `git add .` ajoutera automatiquement tous les fichiers. Vous pouvez faire un `git status` pour voir vos modifications, mais faites-le **avant** `git add`.

7. Validez vos modifications à l'aide d'un message de validation descriptif.
 ```coquille
 git commit -m "Brève description de la validation"
 ```

8. Vérifiez que l'origine est votre propre branche forkée et non le référentiel principal.
 ```coquille
 git distant --verbose
 ```

9. Poussez vos commits sur votre GitHub Fork :
 ```coquille
 git push -u origin votre-nom-de-branche
 ```

10. Soumettez une demande de tirage.
Dans GitHub, visitez ce référentiel principal et vous devriez voir une bannière vous suggérant de faire une pull request. Pendant que vous rédigez la pull request, vous pouvez ajouter « Closes #XXX » dans le corps du message où « #XXX » est le numéro du problème que vous corrigez. Par conséquent, un exemple serait « Ferme #42 » qui fermerait le problème « #42 ».
<br>
<br>


### Ajout d'une nouvelle icône à la page
1. Afin d'ajouter une nouvelle icône à Helpage, vous aurez besoin au préalable des éléments suivants :
 - `LIEN` vers le site Web que vous souhaitez ajouter.
 - Une « IMAGE/SVG » pour le logo du site Web concerné (ou toute image de référence pertinente que vous souhaitez avoir).
2. Téléchargez l'IMAGE/SVG dans le dossier `assets/` avec un nom approprié *(appelons-le ICON_1 par exemple)* et une extension *( **.png**, **.jpg**, ** .jpeg**, **.svg** sont quelques-unes des extensions qui fonctionneront bien)*.
 - Votre fichier doit avoir un chemin relatif similaire à `assets/ICON_1.png` *(Par exemple)*.
3. Une fois que vous avez rassemblé tout ce qui est indiqué ci-dessus et ajouté le logo
 - Ouvrez `Index.html` et recherchez `<AJOUTER UNE ICÔNE ICI>`.
 - Vous devrez décider où exactement vous souhaitez ajouter votre nouvelle icône dans la page et trouver exactement **ce commentaire particulier** `<AJOUTER UNE ICÔNE ICI>`.
4. Copiez et collez les lignes de code suivantes ***sur la ligne JUSTE AU-DESSUS*** du commentaire `<AJOUTER UNE ICÔNE ICI>`.

 ```
 <!-- <AJOUTER UNE ICÔNE ICI> -->

 <!-- <INSÉRER LE NOM> -->

 <div class="col-sm-4 col-4 col-lg-2 col-md-3">
 <div class="icônes dark-elem">
 <a href=" <AJOUTER UN LIEN ICI> " target="_blank">
 <img src="assets/<NOM DE L'IMAGE/SVG>" alt="<ALT TEXT>" height="100px">
 </a>
 </div>
 </div>
 ```
 Mettez à jour les valeurs suivantes en conséquence.
 - `<INSERT NAME>` : Nom du site Web que vous avez lié.
 - `<AJOUTER UN LIEN ICI>` : `LIEN` vers le Site Internet.
 - `<NOM DE L'IMAGE/SVG>` : Nom du fichier Image/SVG du logo ajouté au dossier `assets/` (Pour cet exemple - `ICON_1.png`)
 - `<ALT TEXT>` : Nom du site Web que vous avez lié.

 #### `👌 Vous avez ajouté avec succès une nouvelle icône !! `
<br>
<br>


### Suppression d'une icône existante sur la page
1. Recherchez les commentaires « <AJOUTER UNE ICÔNE ICI> » **Au-dessus et en dessous** de l'icône que vous souhaitez supprimer.
2. Supprimez tout ce qui se trouve entre les deux commentaires.
3. Supprimez **UN** des commentaires `<AJOUTER UNE ICÔNE ICI>`. *(Facultatif mais recommandé)*
#### `👍 Vous avez supprimé avec succès une icône. `
<br>
<br>

### Ajout d'un nouveau signet

1. Recherchez « <AJOUTER UN BOOKMARK ICI> » dans « Index.html ».
2. Copiez et collez les lignes de code suivantes ***sur la ligne JUSTE AU-DESSUS*** du commentaire `<AJOUTER UN BOOKMARK ICI>`.

 ```
 <!-- <AJOUTER UN SIGNET ICI> -->
 <a href="<AJOUTER UN LIEN DE SIGNET>" class="dropdown-item"><INSÉRER LE NOM DU SIGNET></a>
 ```
 Mettez à jour les valeurs suivantes en conséquence :
 - `<AJOUTER UN LIEN BOOKMARK>` : Lien vers le site Web mis en signet.
 - `<INSÉRER LE NOM DU BOOKMARK>` : Nom du site mis en signet.
3. De plus, si vous souhaitez un séparateur de signets, collez la ligne suivante à l'endroit requis.
 ```
 <div class="dropdown-divider"></div>
 ```
#### `👌 Le signet a été ajouté avec succès `
<br>
<br>

### Suppression des favoris existants...
1. Recherchez le commentaire `<AJOUTER UN BOOKMARK ICI>` **Au-dessus et en dessous** du signet que vous souhaitez supprimer.
2. Supprimez tout ce qui se trouve entre les commentaires.
3. Supprimez **UN** des commentaires `<ADD BOOKMARK HERE>`. *(Facultatif mais recommandé)*
#### `👍 Suppression réussie d'un signet `
