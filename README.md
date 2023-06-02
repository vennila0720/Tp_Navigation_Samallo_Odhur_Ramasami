# Tp_Navigation_Samallo_Odhur_Ramasami
#Partie 1: Navigation

La navigation consiste à déplacer le robot d'un endroit à la destination spécifiée dans un environnement donné. À la fin, une carte contenant des informations sur la géométrie des meubles, des objets et des murs de l'environnement donné est requise. Comme décrit dans la section SLAM précédente, la carte a été créée avec les informations de distance obtenues par le capteur et les informations de pose du robot lui-même.


#Etape 1 : 


On a regarde a la page SLAM du E-Manual de Robotis en choisissant noetic et nous nous concentrerons exclusivement sur la méthode de Navigation.
Puis on a exécute le Roscore à partir d'un PC distant.


On a lancée la commande Navigation 

Etape 2 : 

Sur RVIZ,il y a un bouton 2Pose estimate, ce bouton permet de positionner le robot sur la map. 

•	On a clique sur la carte où se trouve le robot réel et faites glisser la grande flèche verte vers la direction à laquelle le robot fait face.
•	Puis on a déplace un peu le robot d'avant en arrière pour collecter les informations sur l'environnement et affiner l'emplacement estimé du TurtleBot3 sur la carte qui est affichée avec de minuscules flèches vertes.
•	Sur RVIZ, il y a un bouton de navigation 2D, ceci permet au robot de se déplacer automatiquement sur la carte. 

Terminez le nœud de téléopération du clavier en entrant Ctrl + C

#Etape 3 : Créer package 

On a crée un  package move_turtle, 
#Etape 4 : on a  utilisée  rviz  et le  bouton  2D  pose  estimate, pour déterminer 3 coordonnées de point où on enverrai le robot .

Le rostopic echo initial pose affiche les messages publiés dans un sujet.

La commande utilisee: roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map_tb5_cleaned_full.yaml

Etape 5: On a ensuite créer un noeud goto.py qui doit faire le robot se deplacer vers une des  coordonnees capturees dans la partie precedente.
