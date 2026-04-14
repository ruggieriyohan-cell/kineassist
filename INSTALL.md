# 🩺 KinéAssist Pro — Guide d'installation

## Fichiers du projet
```
kineassist-pwa/
├── index.html       ← Application principale
├── manifest.json    ← Configuration PWA
├── sw.js            ← Service Worker (cache offline)
└── icons/           ← Icônes de l'app (toutes tailles)
    ├── icon-72.png
    ├── icon-96.png
    ├── icon-128.png
    ├── icon-144.png
    ├── icon-152.png
    ├── icon-192.png
    ├── icon-384.png
    └── icon-512.png
```

---

## 🚀 Déploiement gratuit en 3 minutes (Netlify)

### Étape 1 — Créer un compte gratuit
→ Allez sur **https://netlify.com** et créez un compte gratuit

### Étape 2 — Déployer
1. Depuis le tableau de bord Netlify, cliquez **"Add new site"**
2. Choisissez **"Deploy manually"**
3. **Glissez-déposez le dossier `kineassist-pwa`** dans la zone de dépôt
4. Attendez 30 secondes → votre app est en ligne !

Vous obtenez une URL du type : `https://kineassist-xxxx.netlify.app`

---

## 📱 Installation sur iPhone (iOS)

1. Ouvrez **Safari** sur votre iPhone
2. Tapez l'URL de votre app Netlify
3. Appuyez sur le bouton **Partager** (carré avec flèche ↑)
4. Faites défiler et appuyez sur **"Sur l'écran d'accueil"**
5. Nommez l'app **"KinéAssist"** → **Ajouter**

✅ L'app apparaît sur votre écran d'accueil comme une vraie app !

---

## 📱 Installation sur Android (Chrome)

1. Ouvrez **Chrome** sur votre Android
2. Tapez l'URL de votre app Netlify
3. Chrome affiche automatiquement une bannière **"Ajouter à l'écran d'accueil"**
4. Sinon : menu ⋮ → **"Ajouter à l'écran d'accueil"**
5. Confirmez → l'app est installée !

---

## 🔒 Sécurité des données

- Toutes les données patients sont **chiffrées AES-256-GCM** dans le navigateur
- Stockage **100% local** sur l'appareil (localStorage chiffré)
- **Aucune donnée identifiante** n'est envoyée à un serveur externe
- Seules les données cliniques anonymisées transitent vers l'API d'analyse

---

## ⚙️ Fonctionnement hors ligne

Grâce au Service Worker, l'application **fonctionne partiellement hors ligne** :
- ✅ Interface et données patients accessibles sans internet
- ❌ L'analyse IA nécessite une connexion (API Anthropic)

---

## 🆘 Problèmes fréquents

**"L'app ne s'installe pas sur iPhone"**
→ Assurez-vous d'utiliser Safari (pas Chrome ni Firefox sur iOS)

**"Erreur lors de l'analyse"**
→ Vérifiez votre connexion internet

**"Mes patients ont disparu"**
→ Les données sont liées au navigateur. Ne videz pas le cache de Safari/Chrome.
→ Pour sauvegarder : utilisez toujours le même appareil et navigateur.

---

*KinéAssist Pro — Outil d'aide à la décision clinique*
*Ne remplace pas le jugement professionnel du kinésithérapeute*
