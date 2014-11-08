Plane-Detection-in-Point-Clouds
===============================
Projet INF552 - D�tection de plans dans un nuage de points
===============================


Fonctions � impl�menter
===============================
Impl�mentation d�un octree : partition des nuages pour avoir un faible nombre de plans par bloc

RANSAC : d�tection d�un seul plan

D�finition d�un crit�re d'ambigu�t� sur le nombre de plans

D�finition d�un crit�re de fin de la recherche (pas de plan dans un bloc)

Partition de plans en polygones

Fusion de plans/polygone au-del� des blocs

(Bonus) D�tection d�ar�tes


Structures de donn�es
===============================
-PointCloud : pointeur point -> plan/polygone

-Octree

-Plan :

    vecteur normal + point OU equation (4 coordonn�es) + incertitudes ?

    listes des points issus du RANSAC

-Polygone

    plan d�origine

    listes des points inclus

    enveloppe convexe

    point moyen + rayon pour d�tection de polygones voisins

-(Bonus) Ar�te


Id�es
===============================
-k means

-d�tection de normales locales et croissance


Bibliographie
===============================
data set : http://www.pointclouds.org/news/2013/01/07/point-cloud-data-sets/

github : https://github.com/brandonpelfrey/SimpleOctree

http://www.ipb.uni-bonn.de/fileadmin/publication/pdf/Yang2010Plane.pdf

