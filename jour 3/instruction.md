Une fois que le Dockerfile est fait

Dans le terminal (au niveau du directory): 
- docker build -t imageName . (créer une image)
- docker container run --name containerName -v volumeName:/app/folderName -d --rm -p 3000:80 imageName (créer le container, option --d permet de garder le contrôle sur le terminal, --rm permet de supprimer le container à son arrêt, -p définit le port, ici port 3000 dans le browser expose le port 80 de docker, -v définit le volume)
- docker exec -it containerName bash (permet de rentrer dans le container)