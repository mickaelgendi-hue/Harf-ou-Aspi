# Harf ou Aspi

Deux applications pour apprendre, réunies sur un seul site :

- **Harf** (`arabe/`) : l'arabe **égyptien**. Alphabet et sons, écriture des lettres, lecture, mots et phrases du Caire, dialectes, 64 étapes de cours, 24 types de quiz. Prononciation en **franco** (7 = ح, 3 = ع, 2 = ء/ق, 5 = خ) ou en transcription classique.
- **Aspi** (`copte/`) : le **copte bohaïrique**, uniquement pour **lire et comprendre**. Alphabet, mots, prières et réponses de la messe (vérifiées avec le livret de la messe), 50 étapes de cours, 11 types de quiz.

Un bouton en haut à gauche de chaque application permet de passer de l'une à l'autre.

- Aucune dépendance : chaque application tient dans un seul fichier `index.html`.
- Fonctionne hors ligne après la première visite et peut s'installer sur l'écran d'accueil du téléphone.
- La progression est enregistrée sur l'appareil (dans le navigateur), séparément pour chaque téléphone.

## Structure

```
index.html              page d'accueil (choix Harf / Aspi)
arabe/index.html        Harf — arabe égyptien
copte/index.html        Aspi — copte
manifest.webmanifest    installation sur téléphone
sw.js                   fonctionnement hors ligne
icons/                  icônes de l'application
.github/workflows/      publication automatique sur GitHub Pages
```

## Publier sur GitHub Pages

1. Crée un dépôt GitHub nommé `Harf-ou-Aspi` et envoie-y **tout le contenu de ce dossier** (y compris le dossier caché `.github`).
2. Dans le dépôt : **Settings > Pages > Source : « GitHub Actions »**. Le workflow `.github/workflows/pages.yml` publie le site à chaque envoi sur `main`.
3. Le site sera disponible sur `https://<ton-pseudo>.github.io/Harf-ou-Aspi/`.

Pour mettre à jour : remplace `arabe/index.html` ou `copte/index.html`, puis envoie (commit) les changements.
