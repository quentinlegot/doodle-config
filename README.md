# Doodle Config

Contient tout les fichiers de configurations de doodle

Les dossiers prometheus, front et api contiennent les fichiers de configurations

Le dossier ansible contient les fichiers de déploiements

docker-compose est... le docker-compose mais n'est plus déployé depuis que j'ai terminé l'aventure 7

Le dossier kubernetes contient toutes les confs k8s avec kustomize

Le projet est automatiquement déployer lors d'un push ici, limitant les responsabilités entre le build et les configs (petit rappel des 12 factors)

Les fichiers de build sont ici: [quentinlegot/doodlestudent](https://github.com/quentinlegot/doodlestudent)

Concernant l'aventure 8, j'ai essayé de déployer mais ça ne marchais pas, keycloak n'arrêtais pas de crash en boucle, je l'ai retirer du déployement kustomize et ambassador n'est plus disponible en tant qu'addons sur microk8s depuis la 1.24, les versions récente de ambassador nécessite une licence (pas envie de me créer un compte sur ce site alors que ça va me reservir)