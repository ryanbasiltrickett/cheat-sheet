Cloud Firestore is a flexible, scalable database for mobile, web, and server development from Firebase and Google Cloud. Data in sync across client apps through realtime listeners and offers offline support for mobile and web to build responsive apps that work regardless of network latency or Internet connectivity.

Documentation: [Firebase Firestore Reference](https://firebase.google.com/docs/firestore)
___
## Installation

### On Windows, Linux and macOS
Install Firestore SDK with **Node Package Manager**
```bash
npm install firebase@9.15.0 --save
```

Setup firebase functions with **Firebase CLI ([[Firebase CLI]])**
```bash
firebase init firestore
```

___

## Commands

### Test Firestore Locally
Start and run Firestore locally with **Firebase Emulator ([[Firebase Emulator]])**
```bash
firebase emulators:start
```

___

## Initialize Cloud Firestore

### Initialize Cloud Firestore
Add Firestore to the application to use the integrated features
```javascript
import { initializeApp } from "firebase/app";  
import { getFirestore } from "firebase/firestore";

// Initialize Cloud Firestore and get a reference to the service  
const db = getFirestore(app);
```

### Add Data
Add data to a collection within Firestore, with an auto generated document ID
```javascript
db.collection("collectionName").add({    
	first: "Ada",
	last: "Lovelace",
	born: 1815  
})  
.then((docRef) => {
	console.log("Document written with ID: ", docRef.id);  
})  
.catch((error) => {
	console.error("Error adding document: ", error);  
});
```

Add or overwrite data to a collection within Firestore, with a specified document ID
```javascript
db.collection("collectionName").doc("documentID").set({
	name: "Los Angeles",
	state: "CA",
	country: "USA"  
})  
.then(() => {
	console.log("Document successfully written!");  
})  
.catch((error) => {
	console.error("Error writing document: ", error);  
});
```

### Read Data
Read data from a collection within Firestore
```javascript
db.collection("users").get().then((querySnapshot) => {
	querySnapshot.forEach((doc) => {
		console.log(`${doc.id} => ${doc.data()}`);
	});  
});
```

___