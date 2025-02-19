# Technical Design Document (TDD)

## Table of Contents
1. [Introduction](#1-introduction)

## 1. Introduction

### 1.1 Nom du projet
**Nom du jeu** : _[Portal Dash]_  
**Équipe** : _[GTech3: Gathelier Axel, Enzo Mirabella, Romain Ponsignon, David De Oliveira, Axel Picou; GBS3: GArt2:]_  
**Date de création** : _[18-02-2025]_  
**Version du document** : _[0.1]_  

### 1.2 Objectif du projet
Résumé du concept du jeu : _[...]_

### 1.3 Plateformes et technologies
- **Plateformes cibles** : _[Android, iOS]_  
- **Moteur de jeu** : Unity _[2022.3.32f1]_  
- **Langages de programmation** : C#  
- **Gestion de version** : GitHub _[https://github.com/GamingCampus-MillieBourgois-24-25/grand-projet-commun-portal-dash]_  
- **Autres outils** : _[DoTween, LeanTween, TextMeshPro, Input System, Unity UI, Unity ADs ...]_

---

## 2. Gameplay

### 2.1 Mécaniques de base
- **Type de jeu** : Runner infini
- **Déplacement** : Automatique vers l’avant
- **Contrôles** : _[Swipe gauche/droite, haut/bas, tap ...]_  
- **Obstacles et dangers** : _[...]_
- **Collectibles** : _[...]_

### 2.2 Système de portails
- **Fréquence d’apparition** : _[...]_  
- **Effets possibles** :
  - _[...]_
- **Effets visuels et sonores associés** : _[...]_  
- **Conséquences sur le gameplay** : _[Ex : impact sur la difficulté, ajout de nouvelles mécaniques, ...]_

### 2.3 Power-ups et objets spéciaux
- **Types de power-ups** : _[...]_
- **Durée d’effet** : _[...]_  
- **Méthode d’obtention** : _[...]_  

### 2.4 Système de score et progression
- **Calcul du score** : _[...]_  
- **Multiplicateurs** : _[...]_  
- **Système de missions/objectifs** : _[...]_

---

## 3. Interface Utilisateur (UI/UX)

### 3.1 Éléments du HUD
- **Affichage du score** : _[Où, comment, animation spéciale ...]_  
- **Affichage des power-ups actifs** : _[Icônes, timers, autre...]_  
- **Boutons et interactions** : _[Pause, redémarrer, menu principal, autres...]_  

### 3.2 Menus et navigation
- **Écran titre** : _[...]_  
- **Boutique** : _[...]_  
- **Paramètres** : _[Volume, contrôle sensibilité, graphismes ...]_

---

## 4. Architecture Technique

### 4.1 Organisation du projet Unity
- **Structure des scènes** : _[Scene Menu Principale, Scene Jeu, Scene Ecran de Chargement, Scene Boutique...]_  
- **Système de génération du niveau** : _[...]_  
- **Gestion des assets** : _[...]_  
- **Système de gestion des portails** : _[Comment sont gérés les changements de gameplay?]_  

### 4.2 Performances et optimisation
- **Techniques utilisées** : _[...]_  
- **Ciblage FPS** : _[30FPS, 60FPS, adaptatif?]_  
- **Profiling et test sur mobile** : _[...]_

---

## 5. Plan de Développement

### 5.1 Roadmap
- **Phase 1 : Prototype** (_[Durée prévue]_)  
- **Phase 2 : Core Gameplay** (_[Durée prévue]_)  
- **Phase 3 : Contenu et UI** (_[Durée prévue]_)  
- **Phase 4 : Optimisation et tests** (_[Durée prévue]_)  
- **Phase 5 : Release** (_[Durée prévue]_)  

### 5.2 Répartition des tâches
- **Développeurs** : _[Gathelier Axel, ...]_  
- **Graphistes/UI** : _[Noms et responsabilités]_  
- **Sound Design** : _[Noms et responsabilités]_  
- **Testeurs** : _[Gathelier Axel, ...]_  

---

## 6. Ressources et Références

- **Dépôt GitHub** : _[https://github.com/GamingCampus-MillieBourgois-24-25/grand-projet-commun-portal-dash]_  
- **Outils recommandés** : _[Unity Asset Store, tutoriels, Kenney, Bfxr, ...]_  
- **Documentation technique Unity** : _[...]_  

---

## 7. Notes et Discussions

_(Section pour noter les idées supplémentaires, suggestions d’améliorations ou retours de l’équipe)_
