# mdou-not

Une application mobile pour envoyer des notifications et des messages programmés à des clients via WhatsApp ou des messageries classiques.

## Fonctionnalités

- ✅ **Authentification utilisateur** avec Firebase
- ✅ **Envoi de messages instantanés** via WhatsApp et SMS (Twilio)
- ✅ **Programmation des messages** pour une date/heure spécifique
- ✅ **Gestion des contacts** locaux
- ✅ **Historique d'envoi** avec statut
- ✅ **Interface mobile moderne** avec React Native + Expo

## Technologies utilisées

- **Frontend** : React Native + Expo
- **Backend** : Firebase (Authentification, Firestore)
- **API de messagerie** : Twilio (WhatsApp + SMS)
- **UI Components** : React Native Paper

## Configuration

### Prérequis

- Node.js >= 16
- Npm ou Yarn
- Compte Expo (pour développement et build)
- Compte Firebase
- Compte Twilio

### Installation

1. Clone le repository :
```bash
git clone https://github.com/artistevafoungbe-droid/mdou-not.git
cd mdou-not
```

2. Installe les dépendances :
```bash
npm install
```

3. Configure les variables d'environnement :
```bash
cp .env.example .env
```

4. Remplis le fichier `.env` avec tes clés Firebase et Twilio :
```
EXPO_PUBLIC_FIREBASE_API_KEY=...
EXPO_PUBLIC_FIREBASE_AUTH_DOMAIN=...
EXPO_PUBLIC_FIREBASE_PROJECT_ID=...
EXPO_PUBLIC_FIREBASE_STORAGE_BUCKET=...
EXPO_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=...
EXPO_PUBLIC_FIREBASE_APP_ID=...

EXPO_PUBLIC_TWILIO_ACCOUNT_SID=...
EXPO_PUBLIC_TWILIO_AUTH_TOKEN=...
EXPO_PUBLIC_TWILIO_PHONE_NUMBER=...
EXPO_PUBLIC_TWILIO_WHATSAPP_NUMBER=...
```

### Lancer l'application

#### Sur Expo (développement)
```bash
npm start
```

Scan le code QR avec l'app Expo Go sur ton téléphone.

#### Sur Android
```bash
npm run android
```

#### Sur iOS
```bash
npm run ios
```

## Structure du projet

```
mdou-not/
├── src/
│   ├── context/          # Contextes React (Auth)
│   ├── screens/          # Écrans de l'app
│   ├── services/         # Services (Firebase, Twilio)
│   └── components/       # Composants réutilisables
├── assets/               # Images, icons
├── app.json              # Configuration Expo
├── App.tsx               # Composant principal
└── package.json          # Dépendances
```

## Écrans disponibles

1. **Login** - Connexion avec email/mot de passe
2. **Register** - Création de compte
3. **Home** - Tableau de bord avec accès aux fonctionnalités
4. **Send Message** - Envoi immédiat de SMS/WhatsApp
5. **Schedule Message** - Programmation d'un message
6. **Contacts** - Gestion de la liste de contacts
7. **History** - Historique d'envoi avec statuts

## TODO

- [ ] Intégration complète Firebase Authentication
- [ ] Sauvegarde des contacts dans Firestore
- [ ] Système de programmation backend
- [ ] Notifications push
- [ ] Gestion des tokens de session
- [ ] Tests unitaires
- [ ] Build production APK/IPA

## Contribution

Les contributions sont bienvenues ! N'hésite pas à :

1. Fork le repository
2. Créer une branche (`git checkout -b feature/AmazingFeature`)
3. Commit tes changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

## Licence

MIT - voir le fichier LICENSE

## Support

Pour toute question ou problème, ouvre une issue sur le repository GitHub.

---

**Créé avec ❤️ par artistevafoungbe-droid**