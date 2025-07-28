![Logo](logo.png)

# RÉALISER UN TRAITEMENT BIG DATA DANS UN ENVIRONNEMENT CLOUD

Projet realisé en août 2024 dans le cadre de ma formation Data Scientist avec CentraleSupélec/OpenClassrooms.

## Objectif du projet

L’entreprise "Fruits!" est une très jeune start-up de l'AgriTech qui cherche à proposer des solutions innovantes pour la récolte des fruits. La volonté de l’entreprise est de préserver la biodiversité en permettant des traitements spécifiques à chaque variété en développant des robots cueilleurs intelligents ; elle souhaite dans un premier temps se faire connaître en mettant à disposition du grand public une application mobile qui permettrait aux utilisateurs de prendre en photo un fruit et d'obtenir des informations sur ce fruit. L'objectif pour la start-up est de sensibiliser le grand public à la biodiversité des fruits et de mettre en place une première version du moteur de classification des images de fruits dans un environnement Big Data sur le cloud. En effet, le volume de données va augmenter très rapidement après la livraison du MVP et nécessite la mise en place d’une architecture Big Data elastique (AWS EMR, S3, IAM) utilisant PySpark ainsi qu'un traitement de diffusion des poids du modèle Tensorflow sur les clusters (broadcast des “weights” du modèle). Le respect des contraintes du RGPD sera assuré par un paramétrage de l'installation qui garantit l'utilisation de serveurs situés sur le territoire européen, tout en assurant une gestion optimale des coûts. 


## Liste des fichiers

Les données-source sont disponibles sur https://www.kaggle.com/datasets/moltean/fruits ou en téléchargement direct sur https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/Data_Scientist_P8/fruits.zip.



* **fichiers :**
  - **notebook_1.ipynb :** code Python permettant l'import des fichiers .png et le test du code de transfer learning en local (environnement Windows 10), afin de minimiser les coûts d'utilisation du cluster EMR
  - **notebook_2.ipynb :** code Python transposant le code du notebook_1.ipynb dans l'environnement big data sur AWS EMR
  - **bootstrap_EMR_v700.sh :** fichier de bootstrap pour le cluster EMR
  - **slideshow.pdf :** diapositives de présentation du projet
 


## Compétences développées

 * Modéliser des données dans un environnement Big Data et en utilisant les outils du Cloud
 * Réaliser des calculs distribués sur des données massives en utilisant les outils adaptés
 * Sélectionner les outils du Cloud permettant de traiter et stocker des données Big Data


## Langages & software

 * Python 3.9.13

Voir requirements.txt pour la liste complète des librairies & packages.
  

## MENTIONS LÉGALES

Cette étude a été produite par CelineBoutinon sur la base du jeu de données Fruits-360 dataset sur Kaggle (https://www.kaggle.com/datasets/moltean/fruits). Le jeu de données est fourni « tel quel » et est hébergé sur Kaggle à des fins de recherche et d’éducation ; son utilisation est soumise aux conditions générales de Kaggle ainsi qu’aux termes de la license CC BY-NC-SA 4.0 disponible sur https://creativecommons.org/licenses/by-nc-sa/4.0/.  Les utilisateurs des données sont responsables de l’utilisation qu’ils en font et les analyses présentées ici restent la responsabilité seule de l'auteure. Pour plus de détails, veuillez consulter les conditions d’utilisation sur https://www.kaggle.com/terms et https://www.kaggle.com/docs/datasets#licensing.