> 🔗 Official repository: https://github.com/VeltrixJS/Azarlive-IP-Scanner

# 🔍 Azar IP Scanner

Un script puissant pour analyser les adresses IP en temps réel sur [Azar](https://azarlive.com/) Live avec géolocalisation automatique.

---

## ✨ Fonctionnalités

- 🎯 Détection automatique d'IP via WebRTC
- 🌍 Géolocalisation (Ville, Département, ISP)
- 🚨 Détection VPN/Proxy
- 🗺️ Localisation Google Maps
- 📺 Mode double écran
- 📋 Copie instantanée d'IP

---

## 🚀 Installation

### Méthode 1 : Avec Tampermonkey (Recommandé)

1. **Installer Tampermonkey**
   - [Chrome](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
   - [Firefox](https://addons.mozilla.org/fr/firefox/addon/tampermonkey/)
   - [Edge](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd)

2. **Créer le script**
   - Cliquez sur l'icône Tampermonkey → "Créer un nouveau script"
   - Supprimez tout le contenu par défaut
   - Copiez-collez le contenu de `ip-scanner.js`
   - Sauvegardez (Ctrl+S ou Cmd+S)

3. **Activer le script**
   - Ouvre la page des extensions Chrome en copiant cette adresse dans ta barre de navigation :
```
     chrome://extensions/?id=dhdgffkkebhmkfjojejmpbldmpobfkfo
```
   - Dans les paramètres de Tampermonkey, vérifie que :
     - ✅ La case « Autoriser les scripts utilisateurs » est cochée
     - ✅ Le « Mode développeur » est activé (interrupteur en haut à droite de la page)
   - Le script s'active automatiquement après installation
     
5. **Utiliser**
   - Rendez-vous sur [azarlive.com](https://azarlive.com/)
   - Le panneau apparaît automatiquement en haut à droite
   - Lancez un appel → L'IP s'affiche automatiquement

### Méthode 2 : Console du navigateur

1. Ouvrez [azarlive.com](https://azarlive.com/)
2. Ouvrez la console (**F12** → **Console**)
3. Copiez le contenu de `ip-scanner.js`
4. Collez dans la console
5. **⚠️ Si erreur au collage :** Tapez `allow pasting` directement dans la console, puis recollez le script
6. Appuyez sur **Entrée**

> ⚠️ **Note :** Avec cette méthode, le script se désactive au rechargement de la page. Utilisez Tampermonkey pour une installation permanente.

---
## 🔧 APIs utilisées

### Sans clé API (mode gratuit) - 3 APIs :

1. **ip-api.com** → 45 req/min, géolocalisation + ISP
2. **ipwhois.app** → 10k/mois, détection VPN/Proxy
3. **freeipapi.com** → Pas de limite stricte, détection Proxy

### Avec clé API (optionnel) - 4 APIs :

1. **ipgeolocation.io** → Votre clé API, géolocalisation premium
2. **ip-api.com** → Fallback rapide
3. **ipwhois.app** → Détection VPN/Proxy

> **💡 Système de fallback** : Si une API ne répond pas → passe automatiquement à la suivante.

---

## 🔑 Ajouter une clé API (optionnel)

Pour des limites plus élevées, modifiez la ligne 15 du script :
```javascript
const API_KEY = 'VOTRE_CLE_API_ICI';
```

📝 **Obtenez une clé gratuite** : [ipgeolocation.io/signup](https://ipgeolocation.io/signup.html)


## 📖 Utilisation

### Contrôles

| Bouton | Action |
|--------|--------|
| **📺 2ème écran** | Ouvre une fenêtre popup pour monitoring sur second écran |
| **X** | Minimise l'interface en icône déplaçable |
| **Copy IP** | Copie l'adresse IP dans le presse-papier |
| **Google Maps** | Ouvre la localisation dans Google Maps |

### 💡 Icône Minimisée

- Cliquez sur **X** pour minimiser le panneau
- Une icône apparaît et reste déplaçable
- Cliquez sur l'icône pour rouvrir le panneau au même endroit

## 📷 Aperçu

### Interface principale
<img width="424" height="318" alt="image" src="https://github.com/user-attachments/assets/bb92389f-16ca-479e-8e6c-950652cbabe7" />


### Pop-up second écran 
<img width="431" height="454" alt="image" src="https://github.com/user-attachments/assets/6d5ec5fc-60b7-4179-8c5d-585dae887126" />

## ⚖️ Avertissement légal

Ce projet est fourni **à des fins éducatives et de recherche uniquement**.

- L’auteur n’est pas responsable de l’utilisation abusive de ce script.
- L’utilisation peut être contraire aux conditions d’utilisation d’Azar.
- Respectez les lois locales sur la vie privée et le consentement.

‎ ‎ 
<div align="center">
Made with ❤️ by VeltrixJS
</div>



