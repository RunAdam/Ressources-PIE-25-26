# Simulation et contrôle d'un double pendule monté sur un chariot

Ce dépôt contient l'essentiel des ressources (articles et thèses, codes) jugées pertinentes par l'équipe 24-25.
Il permet de simuler, stabiliser et explorer le contrôle d’un double pendule monté sur un chariot en translation linéaire. 

## Table des matières
- [Structure du dépôt](#structure-du-dépôt)
- [Utilisation](#utilisation)
- [Détails des méthodes](#détails-des-méthodes)
- [Documents disponibles](#documents-disponibles)

---

## Structure du dépôt

Le dépôt est organisé en plusieurs dossiers :

### 1. **`simulation`**
   - **`Sim IHM V2.1.py`**  
     La simulation principale utilisant une intégration de **Runge-Kutta d'ordre 4**.  
     Cette simulation génère des résultats fluides du comportement d’un double pendule monté sur un chariot.
   - **`methode_lqr.py`**  
     Une implémentation de la méthode **LQR (Linear Quadratic Regulator)**.  
     Ce script stabilise le double pendule en position verticale en linéarisant les équations autour de la position d’équilibre.

### 2. **`pilco environment example`**
   - Ce dossier contient un exemple d’environnement pour appliquer l'algorithme **PILCO** (Probabilistic Inference for Learning Control).  
     L’objectif est d’adapter cet algorithme au contrôle du double pendule, mais le projet est encore en cours de développement et **n'est pas encore fonctionnel**.

   Principaux fichiers :
   - `environment.py` : Définit l'environnement personnalisé pour PILCO.
   - `pilco.py` : Contient l'implémentation principale de l'algorithme PILCO.
   - `policy.py` et `utils.py` : Modules d'outils complémentaires.

### 3. **`documentation`**
   - Ce dossier contient des **documents explicatifs** sur :
     - Les bases de la **théorie du contrôle** pour le double pendule.
     - Une introduction et un guide sur **PILCO**.

---

