# Lumi

## Description

  Lumi est un script bash qui utilise Xrandr pour permettre de régler la luminosité de l'écran, en parallèle des réglages du système. 
  
  Il n'est utile que pour les utilisateurs aux yeux sensibles qui veulent baisser la luminosité de leur écran plus bas que le minimum du système.

## Utilisation

  Sous Linux, en ligne de commande.

### Execution

  - Télécharger le fichier "lumi", le rendre exécutable, puis se rendre dans le répertoire du fichier en ligne de commande et passer la commande ```bash lumi```.
  - On peut aussi mettre le fichier dans un répertoire spécifique, et exporter le chemin du dossier dans la variable d'environnement $PATH, afin d'avoir accès à la commande "lumi" de n'importe où. Pour ce faire, passer la commande ```export PATH="/chemin/absolu/vers/répertoire:$PATH"```.
  - Ex: si lumi est dans un dossier "bin" placé dans le dossier utilisateur, passer ```export PATH="$HOME/bin:$PATH"```.

### Arguments

  ```lumi``` peut prendre un argument parmi les suivants :

  ```
    lumi -  # baisse la luminosité de 0,1
    lumi -- # baisse la luminosité de 0,2
    lumi +  # augmente la luminosité de 0,1
    lumi ++ # augmente la luminosité de 0,2
    lumi X  # Passe la luminosité à X (nombre entier ou décimal)
  ```

### N.B.

  De mon expérience, le changement de la luminosité par Xrandr fausse les couleurs de l'écran. Pour cette raison :
  - il n'y a pas vraiment d'intérêt à monter la luminosité au dessus de 1, la valeur par défaut.
  - il n'est pas utile de baisser en dessous de 1 si le réglage de luminosité du système n'est pas déjà au minimum.

### Compatibilité

  Fait pour Linux.
  Testé sous Ubuntu 16, 20, 22 et Manjaro ; devrait marcher sur de nombreuses distributions tant que l'affichage est géré par Xorg.


## A Propos

  Ce petit script est le résultat de mes tout premiers pas vers la programmation, il y a quelques années. Je ne l'ai pas retouché depuis et je m'en sers encore souvent !