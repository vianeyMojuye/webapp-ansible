TP : Déployez un conteneur apache 

1- Créez un cluster (1 ansible et 1 client)

2- Créez un fichier inventaire hosts.yml contenant un groupe prod ayant comme seul membre notre hôte client

3- Créez un dossier grou_vars qui composé du fichier prod.yml qui contiendra les informations de connexion à utiliser par ansible (login et password)

4- Créez un playbook deploy.yml permettant de deployer apache à l'aide de docker sur la machine cliente( image à utiliser est httpd ; port à exposer est 80)

5- utilisez la commande ansible-lint (sudo pip install ansible-lint) : ansible-lint deploy.yml pour vérifier la syntaxe du playbook

6- Explorez les options de debug de ansible avec (-vvv ) : ansible-playbook -i hosts.yml -vvv deploy.yml
