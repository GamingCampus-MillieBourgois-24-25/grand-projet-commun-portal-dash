# Technical Design Document (TDD)

## Table of Contents
1. [Introduction](#1-introduction)
2. [Gameplay](#2-gameplay)
3. [Interface Utilisateur (UI/UX)](#3-interface-utilisateur)
4. [Architecture Technique](#4-architecture-technique)
5. [Plan de Développement](#5-plan-de-developpement)
6. [Ressources et Références](#6-ressoures-et-références)
7. [Nomenclature](#7-nomenclature)

## 1. Introduction

### 1.1 Nom du projet
**Nom du jeu** : _Portal Dash_  
**Équipe** : _GTech3: Gathelier Axel, Enzo Mirabella, Romain Ponsignon, David De Oliveira, Axel Picou_  
**Date de création** : _18-02-2025_  
**Version du document** : _0.4_  

### 1.2 Objectif du projet
Résumé du concept du jeu : _[Un endless runner en 2.5D où le joueur traverse des portails changeant à la fois l'environnement et le gameplay, passant d'un surf dans la neige façon Alto, à un vol triangulaire inspiré de Geometry Dash dans un monde futuriste néon, puis à une course sur des voies ferrées façon Little Big Planet dans une mine.]_

### 1.3 Plateformes et technologies
- **Plateformes cibles** : _[Android, iOS]_  
- **Moteur de jeu** : Unreal Engine _[5.4]_  
- **Langages de programmation** : blueprint / C++
- **Gestion de version** : GitHub _[https://github.com/GamingCampus-MillieBourgois-24-25/grand-projet-commun-portal-dash]_  

---

## 2. Gameplay

### 2.1 Mécaniques de base
- **Type de jeu** : Runner infini
- **Déplacement** : Automatique vers la droite
- **Contrôles** : _Swipe haut/bas, tap_  
- **Obstacles et dangers** : _[...]_
- **Collectibles** : _[...]_

### 2.2 Système de portails
- **Fréquence d’apparition** : _[Aléatoire entre deux valeurs par rapport au score / ou par rapport au temps]_  
- **Effets possibles** :
  - _[...]_
- **Effets visuels et sonores associés** : _[...]_  
- **Conséquences sur le gameplay** : _[Ex : impact sur la difficulté, ajout de nouvelles mécaniques, ...]_

### 2.3 Power-ups et objets spéciaux
- **Types de power-ups** : _[...]_
- **Durée d’effet** : _En fonction du temps en seconde_  
- **Méthode d’obtention** : _Collectable dans les niveaux_  

### 2.4 Système de score et progression
- **Calcul du score** : _Ce calcule par rapport au temps et au multiplicateur temporaire appliqué_  
- **Multiplicateurs** : _[...]_  
- **Système de missions/objectifs** : _[...]_

---

## 3. Interface Utilisateur (UI/UX)

### 3.1 Éléments du HUD
- **Affichage du score** : _En haut à gauche; Score qui s'incrémente en temps réel; Animation sur l'UI lors d'un multiplicateur actif et lors d'un passage de palier de points_  
- **Affichage des power-ups actifs** : _Icônes rondes; Timers visuels sur l'icône (icône affiche le timer sous forme de la perte de couleur de l'asset en fonction du temps et dans le sens de temps)_  
- **Boutons et interactions in-game** : _Bouton pause en haut à droite sous forme d'icône; Interactions avec le jeu en appuyant partout autre que sur le bouton pause_

### 3.2 Menus et navigation
- **Écran titre** : _Bouton regarder une pub pour un bonus; Bouton pour aller dans les paramètres; Bouton invisible au milieu de l'ecran pour lancer la partie (comme Subway Surfer)_  
- **Paramètres** : _Volume (Musique, Bruitage); graphismes (Low, Medium, Hight)_

---

## 4. Architecture Technique

### 4.1 Organisation du projet Unreal Engine
- **Structure des scènes** : _Scene Menu Principale, Scene Jeu, Scene Ecran de Chargement_  
- **Système de génération du niveau** : _[...]_  
- **Gestion des assets** : _[...]_  
- **Système de gestion des portails** : _[Comment sont gérés les changements de gameplay?]_
- **Sytème de sauvegarde** : _Unreal Engine Blueprint_

### 4.2 Performances et optimisation
- **Techniques utilisées** : _[...]_  
- **Ciblage FPS** : _adaptatif_  

---

## 5. Plan de Développement

### 5.1 Roadmap
- **Phase 1 : Prototype de chaque gameplay des portails** (_[Durée prévue]_)  
- **Phase 2 : Ajustement des prototypes et ajouts des gameplay secondaires** (_[Durée prévue]_)  
- **Phase 3 : Ajout de l’UI et des feedbacks** (_[Durée prévue]_)  
- **Phase 4 : Optimisation et tests** (_[Durée prévue]_)  
- **Phase 5 : Release** (_25-04-2025_)  

### 5.2 Répartition des tâches
- **Développeurs** : _Gathelier Axel, David De Oliveira, Axel Picou, Enzo Mirabella, Romain Ponsignon_  
- **Graphistes/UI** : _[Noms et responsabilités]_  
- **Sound Design** : _[Noms et responsabilités]_  
- **Testeurs** : _Gathelier Axel, ..._  

---

## 6. Ressources et Références

- **Dépôt GitHub** : _https://github.com/GamingCampus-MillieBourgois-24-25/grand-projet-commun-portal-dash_  

---

## 7. Nomenclature

### 7.1 Généralités
- Utiliser **PascalCase** pour tous les noms.
- Préfixer chaque asset en fonction de son type pour faciliter l’organisation.
- Éviter les abréviations trop courtes ou non standardisées.
- Utiliser des noms explicites et descriptifs.

### 7.2 Préfixes des assets

| Type d’Asset            | Préfixe  | Exemple                        |
|-------------------------|---------|--------------------------------|
| Blueprint (objet)       | BP_     | `BP_PlayerCharacter`          |
| Blueprint (interface)   | BPI_    | `BPI_Interactable`            |
| Blueprint (fonction utilitaire) | BPF_ | `BPF_MathLibrary`       |
| Matériau                | M_      | `M_PlayerSkin`                |
| Matériau Instance       | MI_     | `MI_PlayerSkinRed`            |
| Texture                | T_      | `T_UI_HealthBar`              |
| Static Mesh            | SM_     | `SM_RockBig`                  |
| Skeletal Mesh          | SK_     | `SK_PlayerCharacter`          |
| Animation Blueprint    | ABP_    | `ABP_Player`                  |
| Séquence d’animation   | ANIM_   | `ANIM_Run`                    |
| Son                   | S_      | `S_Explosion`                 |
| Effet Sonore          | SFX_    | `SFX_PortalOpen`              |
| Musique               | MX_     | `MX_BackgroundTheme`          |
| Particule             | P_      | `P_Explosion`                 |
| Widget                | W_      | `W_MainMenu`                  |
| Niveau (Map)          | LVL_    | `LVL_MainMenu`                |

### 7.3 Blueprints spécifiques
- Les **Blueprints d’acteurs** doivent suivre la structure : `BP_[Nom]`
- Les **Blueprints composants** : `BPC_[Nom]`
- Les **Blueprints de contrôleur** : `BP_Controller_[Nom]`
- Les **Blueprints de GameMode** : `BP_GM_[Nom]`
- Les **Blueprints de HUD** : `BP_HUD_[Nom]`

### 7.4 Variables
- **Booleans** : Préfixe `b` (ex: `bIsJumping`, `bHasPowerUp`)
- **Integers** : `i` (ex: `iScore`, `iHealth`)
- **Floats** : `f` (ex: `fSpeed`, `fJumpHeight`)
- **Vectors** : `v` (ex: `vPlayerPosition`)
- **Textures** : `Tex_` (ex: `Tex_IconPlayer`)
- **Audio** : `Aud_` (ex: `Aud_PortalSound`)
- **Références d’acteurs** : `Ref_` (ex: `Ref_PlayerCharacter`)

### 7.5 Fonctions et événements
- Les fonctions commencent par un verbe pour indiquer l’action : `CalculateScore`, `SpawnEnemy`, `PlaySoundEffect`
- Les événements commencent par `On` : `OnPlayerDeath`, `OnPortalEnter`
- Les macros sont préfixées par `MACRO_` : `MACRO_CalculateDistance`
- Les interfaces sont préfixées par `I_` : `I_Interactable`

### 7.6 Dossiers du projet Unreal
La structure des dossiers doit être claire pour organiser les assets :
