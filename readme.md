# 🎫 ABtime • Wi-Fi Ticket Generator

Générez et distribuez des tickets Wi-Fi sécurisés, chiffrés et à expiration automatique. 100% côté client, sans serveur.

## 📶 Accès Rapide
Scannez ce QR code pour ouvrir l'application directement sur votre téléphone ou tablette :

![QR Code ABtime](https://api.qrserver.com/v1/create-qr-code/?size=400x400&data=https://sellerfit.github.io/wifi-ticket/&bgcolor=ffffff&color=0f172a&margin=10)

🔗 **Lien direct :** `https://sellerfit.github.io/wifi-ticket/`

---

## ✨ Fonctionnalités
- 🔐 **Chiffrement AES-GCM 256 bits** + signature HMAC
- ⏳ **Expiration automatique** configurable (15 min à 24h)
- 🎨 **Personnalisation** : logo, message d'accueil, thème couleur
- 📱 **QR Code universel** compatible iOS & Android
- 🌍 **Multilingue** : Français / English / Español
- 🖨️ **Carte Wi-Fi imprimable** haute définition (PDF vectoriel)
- 📜 **Historique local** & raccourcisseur d'URL intégré

## 🚀 Comment l'utiliser ?
1. Ouvrez le générateur → remplissez le SSID et le mot de passe Wi-Fi.
2. Définissez la durée d'expiration et cliquez sur **Générer**.
3. Partagez le lien ou utilisez la **Carte Wi-Fi / QR** pour l'afficher sur votre comptoir.

## 🛡️ Sécurité & Confidentialité
- Tout le traitement cryptographique s'exécute dans le navigateur (Web Crypto API).
- Aucune donnée sensible (mot de passe, SSID) n'est transmise à un serveur.
- Signature HMAC intégrée pour empêcher la création de faux tickets.
- ⚠️ *Note : L'expiration est vérifiée côté client. Pour une déconnexion réseau forcée, coupliez l'outil à un portail captif (OpenWrt, MikroTik, Ubiquiti...).*

## 📄 Licence & Support
Open Source • Créé par ABtime • 2026  
☕ [Soutenir le projet sur Ko-fi](https://ko-fi.com/sellerfit)
