# firebase-functions-helper
[![Version](https://badge.fury.io/js/firebase-functions-helper.svg)](https://badge.fury.io/js/firebase-functions-helper)
A helper NPM package for Firebase Cloud Functions

## Tables of Contents

* [Installation](#installation)
* [Get Google Cloud Account Credentials from Firebase](#get-google-cloud-account-credentials-from-firebase)
* [Usage](#usage)
* [Contributions](#contributions)

## Installation 

Install using [__npm__](https://www.npmjs.com/).

```sh
npm install firebase-functions-helper
```

## Get Google Cloud Account Credentials from Firebase

You can __Generate New Private Key__ from Project Settings from [Firebase Console](https://console.firebase.google.com).

After that you need to copy the __databaseURL__ for initiating the App. 

## Usage 

### Initialize Firebase App

This is the first step that you need to do before doing any other actions. You still can use the other methods from firebase helpers if you initialize the app by using other methods from Firebase docs.

```sh
const firebaseHelper = require('firebase-functions-helper');
const serviceAccount = require('./serviceAccountKey.json');

// Initialize Firebase App
firebaseHelper.initializeApp(serviceAccount, databaseURL);
```

### [Working with Firestore](docs/firestore.md)
### Working with Realtime Database (Will be updated!)

## Contributions

This project is based on [firebase-functions-snippets](https://github.com/dalenguyen/firebase-functions-snippets), feel free to report bugs and make feature requests in the [Issue Tracker](https://github.com/dalenguyen/firebase-functions-helper/issues), fork and create pull requests!