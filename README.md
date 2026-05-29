# Trading-journal
# 📈 Trading Journal 

Application de journal de trading personnel, installable sur Android et iOS comme une vraie app mobile. Hébergée sur GitHub Pages, sans backend, sans limite de données.

---

## ✨ Fonctionnalités

- Enregistrement de trades (paire, direction, résultat, R:R, émotion, notes)
- Statistiques détaillées : P&L, Win Rate, Profit Factor, Max Drawdown
- Performance par paire de trading
- Export / Import JSON pour sauvegarde complète
- Mode hors-ligne grâce au Service Worker
- Interface sombre, optimisée mobile

---

## 📱 Installation sur téléphone

### Android (Chrome)
1. Ouvrir l'URL GitHub Pages dans **Chrome**
2. Une bannière **"Ajouter à l'écran d'accueil"** apparaît automatiquement
3. Appuyer sur **Ajouter** — l'icône apparaît sur votre écran d'accueil

> Si la bannière n'apparaît pas : menu Chrome `⋮` → **Ajouter à l'écran d'accueil**

### iOS (Safari)
1. Ouvrir l'URL dans **Safari**
2. Appuyer sur le bouton **Partager** `⎙`
3. Sélectionner **"Sur l'écran d'accueil"**
4. Confirmer avec **Ajouter**

---

## 🚀 Déploiement sur GitHub Pages

### Première mise en ligne
1. Créer un repository public sur GitHub
2. Uploader les 5 fichiers suivants :

```
├── index.html
├── manifest.json
├── sw.js
├── icon-192.png
└── icon-512.png
```

3. Aller dans **Settings → Pages**
4. Source : **Deploy from a branch** → branche `main` → dossier `/ (root)`
5. Cliquer sur **Save**

L'application sera accessible à l'adresse :
```
https://<votre-pseudo>.github.io/<nom-du-repo>/
```

### Mettre à jour l'application
1. Modifier le fichier `index.html` sur GitHub (bouton crayon ✏️)
2. Committer les changements
3. GitHub Pages se met à jour automatiquement en quelques secondes

---

## 🗂️ Structure des fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Application complète (HTML + CSS + JS) |
| `manifest.json` | Métadonnées PWA (nom, icône, couleurs) |
| `sw.js` | Service Worker — permet le mode hors-ligne |
| `icon-192.png` | Icône app 192×192 px |
| `icon-512.png` | Icône app 512×512 px |

---

## 💾 Stockage des données

Les données sont stockées localement sur l'appareil via **localStorage** — elles ne transitent jamais par un serveur. Pour ne pas perdre vos trades, utilisez régulièrement la fonction **Export JSON** depuis le menu de l'application.

---

## 🛠️ Technos utilisées

- HTML / CSS / JavaScript vanilla — aucune dépendance
- PWA (Progressive Web App) avec Web App Manifest et Service Worker
- Polices : Space Mono, DM Sans (Google Fonts)
- Hébergement : GitHub Pages (gratuit, illimité)
