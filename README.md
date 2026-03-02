# SSR VSWR Calculator

Application PWA de mesure VSWR pour radar SSR — **YQB & YZV · 1030 MHz**

## Déploiement GitHub Pages

1. Créer un dépôt GitHub (ex: `ssrvswr`)
2. Copier tous les fichiers à la racine du dépôt
3. Activer GitHub Pages : **Settings → Pages → Source → main / root**
4. L'application sera disponible à `https://<username>.github.io/ssrvswr/`

## Structure des fichiers

```
/
├── index.html       — Application principale (tout-en-un)
├── manifest.json    — Manifeste PWA
├── sw.js            — Service Worker (mode hors ligne)
├── .nojekyll        — Désactive Jekyll sur GitHub Pages
└── icons/
    ├── favicon.ico
    ├── icon-72.png  … icon-512.png
```

## Installation sur mobile / desktop

Une fois hébergée, le navigateur proposera automatiquement **« Ajouter à l'écran d'accueil »** (iOS/Android) ou **« Installer »** (Chrome/Edge desktop).

## Fonctionnalités

- Calcul VSWR dynamique — YQB et YZV
- Sélecteur de site avec isolation complète des paramètres
- Table détecteur importable depuis Excel
- Kit d'atténuateurs avec valeurs réelles calibrées
- Statut TI dynamique (seuil 6 mois)
- Export PDF via impression navigateur
- Mode hors ligne (Service Worker)

## Mise à jour du cache

Incrémenter `CACHE_NAME` dans `sw.js` (ex: `ssrvswr-v2`) force le rechargement sur tous les clients.
