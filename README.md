# Technical Design Document (TDD)

## Table of Contents
1. [Introduction](#1-introduction)
2. [Gameplay](#2-gameplay)
3. [Interface Utilisateur (UI/UX](#3-interface-utilisateur)
4. [Architecture Technique](#4-architecture-technique)
5. [Plan de Développement](#5-plan-de-developpement)
6. [Ressources et Références](#6-ressoures-et-références)
7. [Nomenclature](#7-nomenclature)

## 1. Introduction

### 1.1 Nom du projet
**Nom du jeu** : _[Portal Dash]_  
**Équipe** : _[GTech3: Gathelier Axel, Enzo Mirabella, Romain Ponsignon, David De Oliveira, Axel Picou; GBS3: GArt2:]_  
**Date de création** : _[18-02-2025]_  
**Version du document** : _[0.2]_  

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
- **Contrôles** : _[Swipe haut/bas, tap]_  
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
- **Durée d’effet** : _[En fonction du temps en seconde]_  
- **Méthode d’obtention** : _[Collectable dans les niveaux]_  

### 2.4 Système de score et progression
- **Calcul du score** : _[Ce calcule par rapport au temps et au multiplicateur temporaire appliqué]_  
- **Multiplicateurs** : _[...]_  
- **Système de missions/objectifs** : _[...]_

---

## 3. Interface Utilisateur (UI/UX)

### 3.1 Éléments du HUD
- **Affichage du score** : _[En haut à gauche; Score qui s'incrémente en temps réel; Animation sur l'UI lors d'un multiplicateur actif et lors d'un passage de palier de points]_  
- **Affichage des power-ups actifs** : _[Icônes rondes; Timers visuels sur l'icône (icône affiche le timer sous forme de la perte de couleur de l'asset en fonction du temps et dans le sens de temps)]_  
- **Boutons et interactions in-game** : _[Bouton pause en haut à droite sous forme d'icône; Interactions avec le jeu en appuyant partout autre que sur le bouton pause]_

### 3.2 Menus et navigation
- **Écran titre** : _[Bouton regarder une pub pour un bonus; Bouton pour aller dans les paramètres; Bouton invisible au milieu de l'ecran pour lancer la partie (comme Subway Surfer)]_  
- **Paramètres** : _[Volume (Musique, Bruitage); graphismes (Low, Medium, Hight)]_

---

## 4. Architecture Technique

### 4.1 Organisation du projet Unreal Engine
- **Structure des scènes** : _[Scene Menu Principale, Scene Jeu, Scene Ecran de Chargement, Scene Boutique...]_  
- **Système de génération du niveau** : _[...]_  
- **Gestion des assets** : _[...]_  
- **Système de gestion des portails** : _[Comment sont gérés les changements de gameplay?]_
- **Sytème de sauvegarde** : _[Unreal Engine Blueprint]_

### 4.2 Performances et optimisation
- **Techniques utilisées** : _[...]_  
- **Ciblage FPS** : _[adaptatif]_  

---

## 5. Plan de Développement

### 5.1 Roadmap
- **Phase 1 : Prototype de chaque gameplay des portails** (_[Durée prévue]_)  
- **Phase 2 : Ajustement des prototypes et ajouts des gameplay secondaires** (_[Durée prévue]_)  
- **Phase 3 : Ajout de l’UI et des feedbacks** (_[Durée prévue]_)  
- **Phase 4 : Optimisation et tests** (_[Durée prévue]_)  
- **Phase 5 : Release** (_25-04-2025_)  

### 5.2 Répartition des tâches
- **Développeurs** : _[Gathelier Axel, ...]_  
- **Graphistes/UI** : _[Noms et responsabilités]_  
- **Sound Design** : _[Noms et responsabilités]_  
- **Testeurs** : _[Gathelier Axel, ...]_  

---

## 6. Ressources et Références

- **Dépôt GitHub** : _[https://github.com/GamingCampus-MillieBourgois-24-25/grand-projet-commun-portal-dash]_  

---

## 7. Nomenclature

