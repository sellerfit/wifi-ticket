# 🎫 ABtime • Wi-Fi Ticket Generator

Générateur de tickets Wi-Fi sécurisés, 100% client-side, sans backend.

## 🚀 Déploiement (gratuit)

### GitHub Pages (recommandé)
1. Créez un repo `abtime-wifi` sur GitHub
2. Uploadez les 4 fichiers à la racine
3. Allez dans **Settings → Pages → Source: Deploy from branch**
4. Branche: `main`, Dossier: `/ (root)`
5. Votre site sera disponible sur `https://votre-user.github.io/abtime-wifi/`

### Netlify / Vercel
- Glissez-déposez le dossier contenant les 4 fichiers
- Déploiement automatique en < 30 secondes

## 🔐 Sécurité implémentée

| Fonctionnalité | Description |
|---------------|-------------|
| 🔐 AES-GCM 256 | Chiffrement symétrique côté client |
| 🎲 IV aléatoire | Vecteur d'initialisation unique par ticket |
| ✍️ Signature HMAC | Vérification d'intégrité du ticket |
| ⏱️ Expiration | Validation timestamp + avertissement visuel |
| 🌐 HTTPS requis | Les logos personnalisés doivent être en HTTPS |

⚠️ **Limitation** : L'expiration est vérifiée côté client. Pour un usage professionnel critique, ajoutez une validation serveur.

## 🎨 Personnalisation

- ✅ Message de bienvenue personnalisé
- ✅ Logo via URL (HTTPS recommandé)
- ✅ Couleur de thème (sélecteur de couleur)
- ✅ Aperçu en temps réel

## 📜 Historique local

- Sauvegarde automatique dans `localStorage`
- Maximum 20 tickets conservés
- Réutilisation en 1 clic
- Bouton "Effacer tout"

## 🔗 Raccourcisseur d'URL

- Intégration avec [is.gd](https://is.gd) (gratuit, sans API key)
- Fallback automatique vers l'URL longue en cas d'erreur
- Option désactivable dans les paramètres

## 🛠️ Modification

### Changer le secret HMAC (recommandé en production)
Dans `generator.html` et `connect.html`, remplacez :
```js
encoder.encode('ABtime_Secret_2026')