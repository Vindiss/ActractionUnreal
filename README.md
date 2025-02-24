# 🎡 Projet Unreal Engine - Fête Foraine

## 🎮 Description
Ce projet est une simulation de fête foraine créée avec Unreal Engine, offrant plusieurs attractions interactives et des PNJs autonomes. Le joueur peut naviguer en troisième personne et interagir avec différentes attractions ayant leurs propres mécaniques et contrôles spécifiques.

---

## 🚀 Fonctionnalités principales

### 🔹 Game Mode
- Contrôleur à la troisième personne
- Greyboxing (prototypage des niveaux)
- Triggers pour activer les attractions

### 🏃 PNJs Autonomes
- Déplacement aléatoire entre plusieurs points de passage via un NavMesh et des Target Points
- Génération de nouveaux PNJs à l’entrée de la fête foraine selon un taux réglable
- Target point spécial à l’entrée du parc qui fait disparaître les PNJs qui s’y rendent
- Plusieurs types de Target Points (enum) :
  - **Normal** : Positionnement dans un rayon autour de chaque point
  - **Création** : Point de génération
  - **Destruction** : Point de disparition

### 🎯 Attraction Chamboule-Tout
- Caméra à la première personne
- Mécanique de lancé de balle avec force variable
- Boîtes physiques renversables
- Fin de partie après trois essais
- Victoire si plus de la moitié des boîtes sont tombées
- Interface utilisateur : 
  - Jauge de force du lancé
  - Viseur de lancé
- Reset de la position des boîtes à chaque partie

### 🚗 Attraction Auto-Tamponneuses
- Caméra à la troisième personne
- Sélection aléatoire d’un véhicule
- Contrôles spécifiques :
  - `Q/A` : Tourner sur soi-même
  - `Z/S` : Avancer/Reculer
- Véhicule géré par la physique et disparaît s’il est éjecté de la zone de jeu
- Conditions de fin de partie :
  - Timer affiché via un widget
  - Éjection de la zone de jeu
  - Plus de véhicules adverses
- Victoire si le joueur reste dans la zone de jeu jusqu'à la fin


