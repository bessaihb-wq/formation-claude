[README.md](https://github.com/user-attachments/files/27569294/README.md)
# Formation Claude Expert — PWA

Formation interactive Claude API, installable sur téléphone, 100% offline.

## Fichiers

```
formation-claude-pwa/
├── index.html    ← Application complète (cours + quiz)
├── sw.js         ← Service Worker (cache offline)
├── manifest.json ← Config PWA (icône, nom, couleurs)
└── README.md
```

## Déploiement sur GitHub Pages (GRATUIT — 5 minutes)

### Étape 1 — Créer un repo GitHub
1. Aller sur https://github.com/new
2. Nom du repo : `formation-claude` (ou ce que vous voulez)
3. Visibilité : **Public** (requis pour GitHub Pages gratuit)
4. Cliquer "Create repository"

### Étape 2 — Uploader les fichiers
Option A (interface web) :
1. Cliquer "uploading an existing file"
2. Glisser-déposer les 3 fichiers : `index.html`, `sw.js`, `manifest.json`
3. Cliquer "Commit changes"

Option B (ligne de commande) :
```bash
git init
git add .
git commit -m "Formation Claude PWA"
git remote add origin https://github.com/VOTRE_USERNAME/formation-claude.git
git push -u origin main
```

### Étape 3 — Activer GitHub Pages
1. Aller dans Settings → Pages
2. Source : "Deploy from a branch"
3. Branch : `main` / `root`
4. Cliquer Save
5. Attendre 1-2 minutes → votre URL : `https://VOTRE_USERNAME.github.io/formation-claude`

## Installation sur téléphone

### iOS (Safari) :
1. Ouvrir l'URL dans Safari
2. Appuyer sur l'icône Partager ↑
3. "Sur l'écran d'accueil"
4. "Ajouter"

### Android (Chrome) :
1. Ouvrir l'URL dans Chrome
2. Une bannière "Installer l'app" apparaît automatiquement
3. Appuyer sur "Installer"

## Fonctionnalités offline
- ✅ Tous les cours (4 chapitres, 8 sections)
- ✅ Tous les quiz (12 questions)
- ✅ Scores sauvegardés localement (localStorage)
- ✅ Indicateur de mode offline
- ✅ Fonctionne en avion ✈️

## Mise à jour du contenu
Pour modifier les cours/quiz, éditez le tableau `CHAPTERS` dans `index.html`
puis re-déployez sur GitHub (push ou upload).
Le Service Worker se met à jour automatiquement.
