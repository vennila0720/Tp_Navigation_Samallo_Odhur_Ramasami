# Tp_Navigation_Samalloo_Odhur_Ramasami
#Partie 1: Navigation

La navigation consiste à déplacer un robot d'un endroit à la destination spécifiée dans un environnement donné. À la fin, une carte contenant des informations sur la géométrie des meubles, des objets et des murs de l'environnement donné est requise. Comme décrit dans la section SLAM précédente, la carte a été créée avec les informations de distance obtenues par le capteur et les informations de pose du robot lui-même.

#Etape 1: 

En prenant référence à la page SLAM du E-Manual de Robotis et après avoir choisi l'option noetic, nous nous sommes concentrées exclusivement sur la méthode de Navigation.

On a exécuté le Roscore à partir d'un PC distante.

On a ensuite lancée la commande Navigation. 

#Etape 2: 

Sur RVIZ,il y a un bouton nommé 2Pose estimate, ce bouton permet de positionner le robot sur la map. 

•	On a cliqué sur la carte où se trouvait le robot et on a fait glisser la grande flèche verte vers la direction à laquelle le robot faisait face.
•	Puis, on a déplacé le robot d'avant en arrière pour collecter des informations sur l'environnement et affiner l'emplacement estimé du TurtleBot3 sur la carte qui était affichée avec de minuscules flèches vertes.
•	Sur RVIZ, il y a un autre bouton de navigation 2D et celui-ci permet au robot de se déplacer automatiquement sur la carte. 

Terminez le nœud de téléopération du clavier en entrant Ctrl + C

#Etape 3: 

On a crée un package move_turtle

#Etape 4:

On a  utilisée  rviz  et le  bouton  2D  pose  estimate, pour déterminer 3 coordonnées de point où on enverra le robot.

Le rostopic echo initial pose affiche les messages publiés dans un sujet.

La commande utilisee: roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map_tb5_cleaned_full.yaml

#Etape 5:

On a ensuite créer un noeud goto.py qui doit faire le robot se deplacer vers une des coordonnees capturées dans la partie precédente.
