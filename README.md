TP : Déployez un conteneur apache :: Utilisation des Notions templating - loop - condition

1- Créez un cluster (1 ansible et 1 client)

2- Créez un dossier templates avec pour contenu le fichier index.html.j2. Celui-ci devrait permettre l'affichage suivant sur le site:
     binvenue sur - {{nom de l'hôte}}

3- Modifiez le playbook deploy.yml tel que:

     - Utilisez les loop pour installer git et wget à l'aide du module yum

     - Utilisez les conditions afin d'installer wget et git uniquement sur les système CentOs

     -  Modifiez le site internet par defaut, en copiant un template index.html.j2 affichant le message de bienvenue:
           {{nom de l'hôte}} est récupéré dans les variables fournies par ansible
     -  Modifiez le déploiement du conteneur apache afin qu'il monte le fichier index.html dans le repertoire par defaut du site internet apache.
          vous utiliserez la notion de montage de volume
      
4- Vérifiez que votre site est bien conforme aux attentes
 
