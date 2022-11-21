# Exo 2

Créer votre propre dépot gitlab à partir des sources placées dans ce dépôt: https://gitlab.com/cdufour1/cars-api  

Il s'agit des sources d'une API REST réalisée avec le framework java *Spring boot* 

Une fois démarrée, l'application se présente sous forme d'un serveur web exposant un certain nombres de routes (endpoints).   
Ce serveur http écoute par défaut le port _5000_.  
Exemple de route testable: http://localhost:5000/actuator/health  

## tâches
Créer une pipeline avec les phases: deploy, test et deploy.

Suggestion: utiliser pour environnement l'image: *openjdk:12-alpine*  

Commandes utiles
```
# génère en sortie le fichier build/libs/cars-api.jar
gradlew build

# démarre l'application serveur
java -jar ./build/libs/cars-api.jar

# génére le répertoire build/reports/test
gradlew test
```