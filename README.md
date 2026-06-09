# Projet Inscryption
# Description
Ce projet est un jeu crée en Java reproduisant un jeu de cartes au tour par tour inspiré du jeu Inscryption.

# Captures d'écran du jeu
<img width="694" height="791" alt="image" src="https://github.com/user-attachments/assets/9ae0f804-9044-462e-8d3d-047ae60a031d" />

# Installation du projet

# Fonctionnalités de l'application

Face à vous, se trouve un plateau constitué de deux lignes de quatre emplacements de cartes. Vous ne pouvez placer des cartes que sur la ligne du bas, votre adversaire uniquement sur la ligne du haut.

A droite du plateau de jeu, se trouve une balance symbolisant l'écart de score avec votre adversaire. Le premier joueur qui atteint un écart de 5 points en sa faveur remporte la partie.

A votre droite, vous disposez d'une pioche. Vous commencez avec 4 cartes en mains et vous pouvez piocher une carte par tour.

---

**Les cartes animaux**

Chaque carte dispose :
- d'un nombre de points d'attaque
- d'un nombre de points de vie,
- d'un nombre de vos cartes sur le plateau à sacrifier pour pouvoir être placée sur le plateau (nombre de gouttes de sang)
- d'un nombre de vos cartes déjà mortes (tuées ou sacrifiées) pour pouvoir être placée sur le plateau (nombre d'os)

---

**Déroulement d'un tour**

Au début de votre tour, votre adversaire indique quelles cartes il jouera au tour prochain (représentés par une ligne supplémentaire de 4 emplacements de cartes au-dessus du plateau).

A chaque tour, vous pouvez piocher une seule carte que vous placez dans votre main.

Vous pouvez placer autant de cartes de votre main par tour sur le plateau, dans la limite du nombre d'emplacements de cartes disponibles sur votre côté du plateau (au maximum 4) et en respectant les sacrifices à réaliser
A la fin de votre tour, chacune de vos inscryption.cards "animal" attaque. Si une carte de votre adversaire fait face à la carte attaquante, la carte de votre adversaire perd en nombre de points de vie le nombre de points d'attaque de votre carte. 

Si au contraire, aucune carte de votre adversaire ne se trouve face à une de vos cartes, le score est augmenté en votre faveur du nombre de points d'attaque de votre carte. Les cartes "animal" volantes attaquent directement le score même si une carte adverse se trouve en face d'elle.

Les dégâts infligés par les attaques à la fin du tour sont affichés.

Après votre tour, votre adversaire joue de la même façon que vous.

---

**Déroulement de la partie**

Au début de la partie le joueur, prend en main les 4 premières cartes de la pioche.
Des cartes obstacles peuvent être présentes sur le plateau au début de la partie. Elles occupent chacune un emplacement de carte, possèdent un certain nombre de points de vie et doivent être éliminées par vous ou votre adversaire avant de placer une carte à leur emplacement.

La partie se termine lorsqu'un déséquilibre de 5 points apparaît dans le score.

---

**Déroulement du jeu**

Au début de la partie le joueur commence avec une pioche de 15 cartes constituée majoritairement d'écureuils.

Le jeu est constitué de trois parties. Vous gagnez si vous remportez les trois parties.

A la fin de la deuxième partie, vous pouvez ajouter à votre pioche une nouvelle carte parmi les cartes proposées.

A la fin de la deuxième partie, après avoir choisi une nouvelle carte. Le joueur doit sacrifier une carte, il récupère alors son pouvoir (si la carte en possède) et peut l'ajouter à une autre carte animal.

---

**Pouvoirs**

Certains animaux peuvent posséder 1 ou 2 pouvoirs dont :
- Nombreuses vies : reste vivant sur le plateau lorsqu'elle est sacrifiée
- Croissance : se transforme en loup au début du deuxième tour, où il est sur le plateau
- Puant : réduit de 1 l'attaque de la carte lui faisant face
- Coureur : se déplace vers d'un emplacement vers la droite après son attaque. Si l'emplacement vers la droite est bloquée, se déplace vers la gauche. Si les emplacements vers la gauche et la droite sont bloquées ne se déplace pas.
- Contact Mortel: s'il inflige des dégâts à une autre créature (donc pas à un obstacle), la créature blessée meurt
- Piques pointues : inflige 1 point de dégât à la carte attaquante lorsqu'il est attaqué par une carte
