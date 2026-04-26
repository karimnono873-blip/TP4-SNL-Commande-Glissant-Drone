# 🚁 TP4 : Commande par Modes Glissants - Quadricoptère (SMC)

**Institution :** U.S.T.H.B / F.G.E. - Département d'Automatique  
**Module :** Systèmes Non Linéaires (Année universitaire 2025-2026)  
**Auteur :** DAHANE AHMED LAMINE  

---

## 📋 Description du Projet

Ce projet est une application web interactive "Single-Page" (SPA) conçue pour la modélisation, la simulation et le contrôle robuste d'un quadricoptère à 6 degrés de liberté (DDL). Il implémente une architecture de commande hiérarchique basée sur la théorie des **Modes Glissants (Sliding Mode Control - SMC)**.

L'interface "Deep Space Edition" intègre un atelier de câblage interactif, des démonstrations mathématiques professionnelles, un simulateur de vol 3D en temps réel, et le script MATLAB de référence.

## ✨ Fonctionnalités Principales

* **🧠 Atelier de Câblage Intégré :** Un éditeur nodal interactif permettant de connecter virtuellement les blocs du système hiérarchique (Générateur de trajectoire, SMC Position, SMC Attitude, et Dynamique du quadricoptère) pour valider l'architecture.
* **📐 Synthèse Mathématique (MathJax) :** Démonstration typographique propre et lisible des surfaces de glissement et des lois de commande assurant la stabilité au sens de Lyapunov.
* **🕹️ Simulateur 6-DDL (RK4) :** Moteur d'intégration physique embarqué en JavaScript. Permet l'ajustement dynamique des gains de commutation ($K$) et des pentes ($\lambda$) pour observer l'effet sur le *chattering*.
* **🌐 Visualisation 3D :** Rendu spatial interactif de la trajectoire du drone et de sa cible de navigation via Plotly.js.
* **💻 Script MATLAB Officiel :** Fourniture du code source complet incluant la dynamique non linéaire du quadricoptère et la résolution par `ode45`.

## 🚀 Instructions d'Utilisation

L'application fonctionne de manière totalement autonome dans le navigateur, sans installation de logiciels tiers ou de serveurs locaux.

1. **Télécharger** le fichier principal `index.html`.
2. **L'ouvrir** avec un navigateur web moderne (Chrome, Firefox, Edge, Safari).
3. **Câbler** l'architecture dans la section "Atelier de Câblage" en reliant les ports de sortie aux ports d'entrée correspondants jusqu'à validation du système.
4. **Ajuster** les paramètres de vol dans le panneau de contrôle (cibles spatiales $X_d, Y_d, Z_d$ et paramètres d'attractivité SMC).
5. **Lancer la simulation** pour générer et observer la réponse du quadricoptère en 3D.

## 🛠️ Technologies Utilisées

* **Structure & Design :** HTML5, CSS3 (Thème "Deep Space", Glassmorphism, UI/UX Cybernétique).
* **Logique & Simulation :** JavaScript Vanilla (ES6+) pour le moteur Runge-Kutta 4 et la gestion de l'éditeur nodal SVG.
* **Rendu Mathématique :** MathJax pour un affichage vectoriel et optimal des équations.
* **Rendu Graphique 3D :** Plotly.js.

---
*Projet réalisé dans le cadre des travaux pratiques d'ingénierie en automatique.*
