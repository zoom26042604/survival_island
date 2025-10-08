# Survival Island - Jeu de Survie

## Description du Projet

**Survival Island** est un jeu de survie en console développé en Python où vous incarnez un aventurier bloqué sur une île déserte. Votre objectif : gérer vos ressources vitales, faire des choix stratégiques et survivre le plus longtemps possible face aux dangers de l'île.

## Règles du Jeu

### Jauges Vitales

Votre aventurier possède trois jauges à surveiller constamment :

- **Faim** (0-100) : Plus la valeur est élevée, plus vous avez faim
  - 0 = Rassasié
  - 100 = Affamé → **GAME OVER**

- **Soif** (0-100) : Plus la valeur est élevée, plus vous êtes assoiffé
  - 0 = Hydraté
  - 100 = Déshydraté → **GAME OVER**

- **Énergie** (100-0) : Votre niveau d'énergie diminue avec vos actions
  - 100 = Pleine forme
  - 0 = Épuisé → **GAME OVER**

### Mécaniques de Jeu

#### Évolution Naturelle
Chaque jour, vos jauges évoluent automatiquement :
- La faim augmente
- La soif augmente
- L'énergie diminue légèrement

#### Actions Disponibles

Chaque jour, vous pouvez effectuer **une action** parmi :

1. **Pêcher**
   - Diminue la faim
   - Consomme de l'énergie

2. **Chercher de l'eau**
   - Réduit la soif
   - Consomme de l'énergie

3. **Dormir**
   - Remonte l'énergie
   - Augmente légèrement la faim et la soif

4. **Explorer**
   - Déclenche un événement aléatoire
   - Peut être bénéfique ou dangereux
   - Consomme de l'énergie

#### Événements Aléatoires

Au cours de votre survie, vous pouvez rencontrer :
- **Pluie** : Réduit votre soif automatiquement
- **Animaux sauvages** : Choisissez de fuir ou de chasser
- **Découverte de nourriture** : Fruits, baies, ressources
- **Dangers divers** : Blessures, épuisement, etc.

### Conditions de Fin

#### Game Over
La partie se termine si :
- La faim atteint 100
- La soif atteint 100
- L'énergie tombe à 0

#### Victoire
Survivez un nombre de jours prédéfini (par exemple 30 jours) pour gagner !

## Installation et Lancement

### Prérequis
- Python 3.7 ou supérieur
- Aucune bibliothèque externe requise (utilise uniquement la bibliothèque standard Python)

### Installation

1. Clonez le dépôt :
```bash
git clone https://github.com/zoom26042604/survival_island.git
cd survival_island
```

2. Vérifiez votre version de Python :
```bash
python --version
```

### Lancement du Jeu

Exécutez le programme principal :
```bash
python src/main.py
```

Ou depuis la racine du projet :
```bash
python -m src.main
```

## Fonctionnalités

### Sauvegarde et Chargement
- **Sauvegarde automatique** : Vos progrès sont enregistrés régulièrement
- **Chargement** : Reprenez votre partie là où vous l'avez laissée
- Format de sauvegarde : JSON (fichier `saves/savegame.json`)

### Système de Statistiques
- Nombre de jours survécus
- Actions effectuées
- Événements rencontrés
- Score final

## Structure du Projet

```
survival_island/
│
├── src/
│   ├── main.py          # Point d'entrée du jeu
│   ├── game.py          # Logique principale du jeu
│   ├── player.py        # Classe du joueur et gestion des jauges
│   ├── events.py        # Système d'événements aléatoires
│   └── utils.py         # Fonctions utilitaires
│
├── saves/               # Dossier des sauvegardes
│   └── savegame.json
│
├── assets/              # Ressources (textes, configurations)
│
├── README.md            # Ce fichier
└── LICENSE              # Licence du projet
```

## Stratégies de Survie

### Conseils pour Débutants
1. **Équilibrez vos actions** : Ne négligez aucune jauge
2. **Dormez régulièrement** : L'énergie est cruciale
3. **Explorez avec prudence** : Les événements peuvent être dangereux
4. **Profitez de la pluie** : Événement gratuit qui réduit la soif

### Stratégies Avancées
- Anticipez l'évolution de vos jauges
- Prenez des risques calculés avec l'exploration
- Gérez votre énergie pour pouvoir agir en cas d'urgence

## Auteurs

Projet développé en binôme par :
- FERRE Nathan
- BARREAU Romain

## Licence

Ce projet est sous licence [MIT](LICENSE).

## Bugs Connus et Améliorations Futures

### Améliorations Prévues
- Système de craft d'objets
- Différents niveaux de difficulté
- Plus d'événements aléatoires
- Interface graphique (GUI)
- Système d'achievements
- Multiplicateurs de score

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
1. Fork le projet
2. Créer une branche (`git checkout -b feature/amelioration`)
3. Commit vos changements (`git commit -m 'Ajout d'une fonctionnalité'`)
4. Push vers la branche (`git push origin feature/amelioration`)
5. Ouvrir une Pull Request

## 📞 Contact

Pour toute question ou suggestion :
- Email :  [ nathanferre@gmail.com & romain.barreau31@gmail.com ]

---

**Bon courage et bonne survie sur l'île !**
