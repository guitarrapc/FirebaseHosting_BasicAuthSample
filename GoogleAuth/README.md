## FirebaseHosting_BasicAuthSample

## Getting started ✈️

1. Create Firebase Project at https://console.firebase.google.com
1. Install firebase-tools `npm install -g firebase-tools`
1. Login to firebase project `firebase login`
1. Initialize for your firebase project. `firebase init`
1. Get api info from https://console.firebase.google.com/project/<PROJECT_NAME>/settings/general/ and input project info inside `public/js/config.js`.
1. set your restricted domain by `AuthUI.provider.setCustomParameters` in side `public/js/basicAuth.js`
1. Deploy! `firebase deploy`

## How to modify 📝

* If you don't restrict user domain, setCustomParameters section.
```javascript
AuthUI.provider.setCustomParameters({
    'hd': "YOUR_DOMAIN.com"
});
```
