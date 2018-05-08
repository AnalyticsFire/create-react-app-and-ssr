# Create React App + Server Side Rendering

## Setup

```
git clone git@github.com:analyticsfire/create-react-app-and-ssr.git
cd icr-front-end
yarn install
```

## Install cra-universal (Create React App + Server Side Rendering)

Simple express server for your Create React App projects with Server-side rendering and Code-splitting.

Why you must use this?

- No eject needed!
- Server-side rendering for your SEO
- Code-splitting that works universally
- Server code is given to you, no black-box
- The core middleware is fully unit-tested

Sources: 
- Doc: https://medium.com/@antonybudianto/cra-universal-universal-create-react-app-without-ejecting-f50d4d179261
- Npm: https://www.npmjs.com/package/cra-universal
- Github: https://github.com/antonybudianto/cra-universal

### Installation

```
# Install global CLI 
npm install -g cra-universal
```

## How to run development

```
cra-universal start
```

This will run both CRA client and server dev-server.

You can visit `http://localhost:3001` for the server-side rendered version, and `http://localhost:3000` for the client-side rendered version (the usual CRA).

Now try to use curl to check whether you get the full rendered version or not

## How to deploy your app

```
cra-universal build
```

This will build both the client and server bundle and put them together into dist folder. You can deploy dist into your Nodejs server, like now.sh, Firebase functions, or even your own server instance.

## How to clean up the build results

```
cra-universal clean
```
