# Jekyll-Firebase

A Jekyll Site with support for user login via Firebase. This means you can run a static site on GitHub Pages and still support some basic login functionality, by outsourcing all of your sign in and storage of user data to Firebase.

Firebase supports login using email, Google, Facebook, Twitter, GitHub, or anonymously.



## Setup

For this site to work correctly you will need to:

- Create a Firebase account and project
- Modify the `firebase-config.js` file with your own details
- Authorise your site's domain



## Authorise Your Domain

Firebase needs to know which domain you are running your site on.

1. Open the Firebase Console for your project
2. Click "Auth" in the sidebar
3. Click the "Sign in Method" tab
4. Under "OAuth redirect domains" add your domain

If your domain is not authorised correctly the UI will stay loading until it times out, and you will get the following error in your JavaScript console:

_"The current domain is not authorized for OAuth operations. This will prevent signInWithPopup, signInWithRedirect, linkWithPopup and linkWithRedirect from working. Add your domain to the OAuth redirect domains list in the Firebase console -> Auth section -> Sign in method tab."_