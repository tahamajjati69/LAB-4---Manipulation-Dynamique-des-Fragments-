# Android Java – Gestion des Fragments

## 📖 Description
Ce projet Android Java illustre l’utilisation des **Fragments** pour créer une interface dynamique et réutilisable.  
L’application permet de basculer entre deux fragments :
- **FragmentOne** : affiche un texte et un bouton pour interagir.
- **FragmentTwo** : contient une barre de progression (`SeekBar`) et conserve son état lors des changements.

---

## 📂 Structure du projet
```
app/
└── src/
└── main/
├── java/com/example/fragmentslab/
│   ├── MainActivity.java
│   ├── FragmentOne.java
│   └── FragmentTwo.java
└── res/
    └── layout/
        ├── activity_main.xml
        ├── fragment_one.xml
        └── fragment_two.xml
```

## ⚙️ Fonctionnalités
- **MainActivity** :
  - Contient deux boutons pour charger les fragments.
  - Méthode `replaceFragment()` pour remplacer dynamiquement le fragment affiché.
  - Gestion du `BackStack` pour naviguer entre les fragments.

- **FragmentOne** :
  - Affiche un `TextView` et un bouton.
  - Lors du clic, le texte change en : *"Bonjour depuis Fragment 1 !"*.
  - Journalisation du cycle de vie (`onResume`, `onPause`).

- **FragmentTwo** :
  - Affiche un `SeekBar` et un `TextView` indiquant la valeur.
  - Sauvegarde et restauration de l’état (`onSaveInstanceState`).
  - Mise à jour dynamique du texte lors du déplacement du curseur.

---

## 🖥️ Exemple d’exécution


https://github.com/user-attachments/assets/b1e214b6-5bab-42d1-a361-d6f333bc8ce5



---
## 💡 Concepts pratiqués
- Utilisation des **Fragments** pour modulariser l’interface.
- Gestion du cycle de vie des fragments (`onResume`, `onPause`).
- Sauvegarde/restauration de l’état avec `Bundle`.
- Navigation dynamique avec `FragmentManager` et `FragmentTransaction`.
- Interaction utilisateur via `Button` et `SeekBar`.

---

## 🧑‍💻 Auteur
👤 **Majjati Mohamed Taha**  
📱 Développement Android Java  
🎓 Instructor : **Mr. LACHGAR**  
📅 14 Mars 2026
