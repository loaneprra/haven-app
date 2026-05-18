# Haven 🛡️

**Voyager libre. Voyager safe.**

Application de sécurité pour voyageuses solo en Thaïlande.

## 🚀 Déploiement sur Netlify

### Option 1 : Déploiement automatique via Git

1. Créez un compte sur [Netlify](https://www.netlify.com/)
2. Connectez votre repository GitHub/GitLab
3. Netlify détectera automatiquement la configuration dans `netlify.toml`
4. Le site sera déployé automatiquement à chaque push

### Option 2 : Déploiement manuel

1. Générez le build de production :
   ```bash
   pnpm install
   pnpm run build
   ```

2. Le dossier `dist/` contient l'application prête pour le déploiement

3. Uploadez le dossier `dist/` sur Netlify :
   - Via l'interface web : glissez-déposez le dossier `dist/` sur Netlify
   - Via Netlify CLI : 
     ```bash
     npm install -g netlify-cli
     netlify deploy --prod --dir=dist
     ```

## 📦 Build de production

Le build est configuré avec :
- ✅ Chemins relatifs (`base: './'`) pour compatibilité Netlify
- ✅ Fichier `_redirects` pour React Router
- ✅ Optimisation et minification automatique
- ✅ Taille totale : ~719 KB

## 🛠️ Technologies

- **Framework** : React 18.3 + TypeScript
- **Routing** : React Router 7
- **Styling** : Tailwind CSS v4
- **Maps** : Leaflet + React Leaflet
- **Icons** : Lucide React
- **Build** : Vite 6

## 📱 Fonctionnalités

- 🆘 Bouton SOS avec compte à rebours
- 🗺️ Safe Map avec zones sécurisées
- 👩‍👩‍👧 Communauté de voyageuses
- 📊 SafeScore en temps réel
- 🌏 Ressources culturelles et formations
- ♿ Accessibilité complète (vision, dys, navigation)
- 📲 PWA-ready avec support mobile optimisé

## 🔧 Développement local

```bash
# Installation
pnpm install

# Développement
pnpm run dev

# Build de production
pnpm run build

# Preview du build
pnpm run preview
```

## 📄 License

© 2026 Haven - Tous droits réservés
