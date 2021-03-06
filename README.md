# RetroMatic

[![Build Status](https://travis-ci.org/wordythebyrd/agile-retrospective.svg?branch=master)](https://travis-ci.org/wordythebyrd/agile-retrospective)
[![Latest Version](https://img.shields.io/github/tag/wordythebyrd/agile-retrospective.svg)](https://github.com/wordythebyrd/agile-retrospective)

![RetroMatic](src/assets/Images/rmbg.jpg)

RetroMatic is a web appplication used to conduct **retrospectives**.  A retrospective is a meeting that's held at the end of an iteration in **Agile** software development. During the retrospective, the team reflects on what happened in the iteration and identifies actions for improvement going forward.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* Install Angular CLI.  This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.3.2.

```bash
# Install Angular CLI
$ npm install -g @angular/cli
```

* Create a [Firebase](https://firebase.google.com/) project and install the Firebase CLI.  In Firebase console, enable Email/Password, Google, and Anonymous sign-in under the sign-in method tab of the Auth section.

```bash
# Install Firebase CLI
$ npm install -g firebase-tools
```

### Installing

To clone and run this application, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/wordythebyrd/agile-retrospective.git

# Go into the repository
$ cd agile-retrospective

# Install dependencies
$ npm install
```
Update firebase config values in `firebase.ts`.  This config file will be ignored from GIT. Copy `firebase.example.ts` and rename it to `firebase.ts`. These values can be found here: Firebase Console > Overview > Add Firebase to your web app.

```javascript
    firebase: {
        apiKey: '',
        authDomain: '',
        databaseURL: '',
        projectId: '',
        storageBucket: '',
        messagingSenderId: ''
    }
```


```bash
# Run the app
$ ng serve
```
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

```bash
$ ng test
```
Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

```bash
$ ng e2e
```

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.