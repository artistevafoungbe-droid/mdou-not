# Guide d'Installation - mdou-not

## 📋 Prérequis

- **Node.js** >= 16.x (télécharger depuis https://nodejs.org/)
- **npm** ou **yarn** (inclus avec Node.js)
- **Expo CLI** (optionnel mais recommandé)
- **Compte Firebase** (https://console.firebase.google.com/)
- **Compte Twilio** (https://www.twilio.com/)

## 🚀 Étapes d'installation

### 1. Cloner le repository
```bash
git clone https://github.com/artistevafoungbe-droid/mdou-not.git
cd mdou-not
```

### 2. Installer les dépendances
```bash
npm install
```

Ou avec yarn :
```bash
yarn install
```

### 3. Configurer les variables d'environnement

Copier le fichier `.env.example` en `.env` :
```bash
cp .env.example .env
```

Remplir le fichier `.env` avec vos données :

#### Configuration Firebase
1. Aller sur https://console.firebase.google.com/
2. Créer un nouveau projet
3. Aller dans "Paramètres du projet" → "Clés d'API"
4. Copier les informations :

```
EXPO_PUBLIC_FIREBASE_API_KEY=votre_api_key
EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=votre_project.firebaseapp.com
EXPO_PUBLIC_FIREBASE_PROJECT_ID=votre_project_id
EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=votre_project.appspot.com
EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=votre_sender_id
EXPO_PUBLIC_FIREBASE_APP_ID=votre_app_id
```

#### Configuration Twilio
1. Aller sur https://www.twilio.com/
2. Créer un compte
3. Récupérer votre ACCOUNT SID et AUTH TOKEN
4. Acheter un numéro de téléphone pour SMS
5. Paramétrer WhatsApp Business

```
EXPO_PUBLIC_TWILIO_ACCOUNT_SID=votre_account_sid
EXPO_PUBLIC_TWILIO_AUTH_TOKEN=votre_auth_token
EXPO_PUBLIC_TWILIO_PHONE_NUMBER=+237xxxxxxxxx
EXPO_PUBLIC_TWILIO_WHATSAPP_NUMBER=+237xxxxxxxxx
```

### 4. Vérifier l'installation

```bash
npm start
```

Vous devriez voir :
```
expo-cli started successfully
To open your app in Expo Go, scan the QR code below
```

## 📱 Lancer l'application

### Sur Expo Go (Recommandé pour le développement)
```bash
npm start
```

Scannez le code QR avec l'app Expo Go (disponible sur iOS App Store et Google Play)

### Sur Android
```bash
npm run android
```

### Sur iOS
```bash
npm run ios
```

## ⚠️ Troubleshooting

### Port 8081 déjà utilisé
```bash
npx expo start --clear
```

### Erreur Firebase "Config is not a valid Firebase config"
- Vérifier que le fichier `.env` est correct
- S'assurer que les clés Firebase sont valides
- Redémarrer l'application

### Erreur "Module not found"
```bash
rm -rf node_modules package-lock.json
npm install
```

## 📚 Documentation utile

- [Expo Documentation](https://docs.expo.dev/)
- [Firebase Documentation](https://firebase.google.com/docs)
- [Twilio Documentation](https://www.twilio.com/docs)
- [React Navigation](https://reactnavigation.org/)

## ✅ Vérifier que tout fonctionne

1. L'app se lance sans erreur
2. Vous pouvez créer un compte avec Firebase
3. Vous pouvez vous connecter
4. L'écran d'accueil s'affiche

Si tout cela fonctionne, l'installation est réussie ! 🎉

---

**Besoin d'aide ?** Consultez le fichier README.md ou ouvrez une issue sur GitHub.
