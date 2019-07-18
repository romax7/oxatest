# Utiliser un service de stockage externe
Nous allons voir pas à pas comment heberger ses scripts sur une platforme externe à Oxatis.
Nous verrons Google cloud Storage //et Amazon web service (pas encore)//.

## Google cloud storage
Dans google cloud, vous avez la possibilité de créer une multitude de chose. Nous allons nous interesser à google cloud storage qui est un moyen simple de stocker des fichiers de toute nature.

### Se connecter
Afin d'utiliser google cloud, il est necessaire d'avoir un compte google.
Pour ce faire, rendez vous sur [cloud.google.com](https://cloud.google.com/).

Pour tous les nouveaux inscrits, google offre 300$ de crédit à utiliser pendant 1 an.

![Image Connexion](img/start-google.png)

Une fois connecté, vous devez accepter les conditions d'utilisation, remplir tous les champs et préciser un moyen de paiement (même si vous disposez d'un essaie gratuit d'une durée de un an, le moyen de paiement doit être précisé).

## Créer un projet
Avant de créer un espace de stockage, il est necessaire de créer un projet.
Pour ce faire, cliquez sur créer un projet (voir image ci-dessous)

![Image create project](img/create-project.png)

Définissez un nom pour votre projet 
**Attention ! Vous ne pourrez pas le modifier**
Et choisissez une "zone" si vous le souhaitez.

![Image create project](img/create-project-2.png)

Une fois votre projet créé, vous allez alors être redirigé vers le *dashboard* du projet. 

![Image create project](img/dashboard-project.png)

Maintenant que vous avez un prjet, nous allons créer un espace de stockage. Nous le nomerons *bucket*. C'est là où vous mettrez vos fichiers. Pour ce faire, ouvrez le menu de gauche (voir image ci-dessous) et selectionnez "*stockage*" dans le menu.

![Image create project](img/dashboard-stockage.png)

Une fois dans la page stockage, cliquez sur créer un bucket (voir image ci-dessous).

![Image create project](img/create-bucket.png)

Après suivez les étapes ci-dessous.
Tout d'abord, donnez un nom à votre bucket. Nous nous servirons de ce nom plus tard.

![Image create project](img/create-bucket-1.png)

Choisissez "Multi-regional" et choisissez une zone (de préférence proche de vos clients).

![Image create project](img/create-bucket-2.png)

Ensuite, choisissez "Définir des autorisations au niveau de l'objet et du bucket".

![Image create project](img/create-bucket-3.png)

Ensuite, ne touchez à rien et laissez les valeurs par défaut.
Cliquez sur "créer" pour créer votre bucket.

![Image create project](img/create-bucket-4.png)

Et voila votre bucket de stockage est maintenant créé. Vous pouvez y ajouter des fichiers directement depuis l'interface google cloud mais nous verrons plus tard comment automatisé les accés au bucket.

![Image create project](img/create-bucket-5.png)
