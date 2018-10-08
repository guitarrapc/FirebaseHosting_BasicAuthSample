## FirebaseHosting Cloud Functions Basic Auth Sample

## Getting started ✈️

1. Create Firebase Project at https://console.firebase.google.com
1. Install firebase-tools `npm install -g firebase-tools`
1. Login to firebase project `firebase login`
1. Initialize for your firebase project. `firebase init`
1. Deploy! `firebase deploy`

## How to modify 📝

/auth is hosting firebase functinos.

* `public/index.html` : content root.
* `functions/index.js` : cloud functions to provide basic authentication.
* `firebase.json` : firebase routing rules.
    * `rewrites` section indicate url `/auth` pass request to authenicate cloud function.
    * `redirects` section indicate `/` will redirect to `/auth`. So when you access to site 

## Restriction 🙅

* This method cannot restrict direct .html acess. For example, /index.html can see without authentication.