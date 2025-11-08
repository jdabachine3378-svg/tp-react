---
title: TP React – Application de Gestion des Composants
author: Jamila Dabachine — ENS Marrakech
description: Projet React illustrant la création et l’utilisation de composants, de props et de PropTypes. Réalisé dans le cadre du Master “Technologies Émergentes en Éducation”.
version: 1.0
date: Novembre 2025
---
# 🎓 TP React – Application de Gestion des Composants
#  **🎯 Objectif du TP
L’objectif de ce TP est d’apprendre à créer, structurer et utiliser plusieurs composants React au sein d’une même application.
Les principaux points abordés sont :

Création de composants fonctionnels

Utilisation des props pour transmettre des données

Validation des données via PropTypes

Organisation de l’arborescence d’un projet React

# ⚙️ Étapes d’installation et d’exécution
# 1️⃣ Création du projet
bash
Copier le code
npx create-react-app tp-react
cd tp-react
# 2️⃣ Lancement du serveur
bash
Copier le code
npm start
# ➡️ L’application sera accessible sur : http://localhost:3000

# 📁 Structure du projet :
<img width="581" height="795" alt="image" src="https://github.com/user-attachments/assets/65df923e-0d46-4680-a144-8c091b045314" />


#  Ce composant affiche simplement :

jsx
Copier le code
<h1>Hello World!</h1>
🔹 Greeting.js
Ce composant reçoit un prénom via props et affiche :

jsx
Copier le code
Bonjour, {prenom} !
🔹 Profil.js
Affiche un profil utilisateur avec une image et un nom :

jsx
Copier le code
<img src={utilisateur.photo} width={taille} alt={utilisateur.nom} />
<p>{utilisateur.nom}</p>
🔹 Voiture.js
Affiche les caractéristiques d’une voiture :

jsx
Copier le code
Voiture : {marque} {modele}, Couleur : {couleur}
🔹 ListeCourses.js
Affiche une liste de courses passée sous forme de tableau :

jsx
Copier le code
<ul>
  {elements.map((element, index) => (
    <li key={index}>{element}</li>
  ))}
</ul>
# 🖼️ Captures d’écran
<img width="1179" height="576" alt="Capture d’écran 2025-11-08 160611" src="https://github.com/user-attachments/assets/60ccccd1-55c9-431f-901b-ca929dd9e87c" />
<img width="1014" height="485" alt="Capture d’écran 2025-11-08 160823" src="https://github.com/user-attachments/assets/d16fcca0-263a-463e-ab66-027539494eb5" />
<img width="716" height="531" alt="Capture d’écran 2025-11-08 162845" src="https://github.com/user-attachments/assets/ae2e2fd4-e271-4d49-8203-b626cb042034" />

# 🚀 Résultat final
L’interface de l’application présente :

Un message Hello World!

Deux messages de bienvenue : Bonjour Alice et Bonjour Mohamed

Un profil utilisateur nommé Emma avec sa photo

Une liste de voitures (Toyota, Peugeot, Renault)

Deux listes de courses 🛒

# 🧠 Technologies utilisées
React 18.x

Node.js 22.x

Babel / JSX

PropTypes

NPM

#  📚 Bonnes pratiques appliquées
Composants séparés pour une meilleure lisibilité

Validation des props pour éviter les erreurs

Utilisation de fragments <> ... </> pour grouper plusieurs éléments JSX

Structure de projet claire et modulable

# 👩‍💻 Auteur
Jamila Dabachine — ENS Marrakech
Master Technologies Émergentes en Éducation
📅 Novembre 2025


# 🏁 Conclusion
Ce projet montre comment créer une petite application React structurée en plusieurs composants indépendants.
C’est une base solide pour comprendre la logique de React et la communication entre les composants via les props.

