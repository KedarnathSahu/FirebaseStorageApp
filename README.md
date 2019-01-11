# FirebaseStorageApp
Uploading and Retrieving Images - [Firebase: (Storage + Realtime Database)]

# Storage Rules

service firebase.storage {
  match /b/{bucket}/o {
    match /{allPaths=**} {
      allow read, write: if true ;//request.auth != null 
    } 
  } 
}

# Realtime Database Rules

{
  /* Visit https://firebase.google.com/docs/database/security to learn more about security rules. */
  "rules": {
    ".read": true,
    ".write": true
  }
}

<img src="https://s2.gifyu.com/images/ezgif.com-resizeffeeb86e85560dda.gif"/>
