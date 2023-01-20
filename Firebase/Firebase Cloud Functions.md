Cloud Functions for Firebase is a serverless framework that lets you automatically run backend code in response to events triggered by Firebase features and HTTPS requests. JavaScript or TypeScript code is stored in Google's cloud and runs in a managed environment. 

Documentation: [Firebase Functions Reference](https://firebase.google.com/docs/functions)
___

## Installation and Setup

### On Windows, Linux or macOS
Setup firebase functions with **Firebase CLI ([[Firebase CLI]])**
```bash
firebase init functions
```

___

## Commands

### Test Functions Locally
Start and run functions endpoint with **Firebase Emulatore ([[Firebase Emulator]])**
```bash
firebase emulators:start
```

### Deploy Functions to Firebase
Deploy **All** functions to Firebase to use them from firebase endpoint
```bash
firebase deploy --only functions
```

Deploy a **specififc** function to Firebase to use from firebase endpoint
```bash
firebase deploy --only functions:functionName
```

___
