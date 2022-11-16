# Berith-IDE

## Berith IDE
**Berith IDE** has been forked from [remix project v0.28](https://remix.ethereum.org) for smart contract distribution to Berith-chain, and is fully compatible with Berith-chian's account prefix 'Bx'.

## Remix Project
**Remix Project** is a rich toolset including Remix IDE, a comprehensive smart contract development tool. The Remix Project also includes Remix Plugin Engine and Remix Libraries which are low-level tools for wider use.  

## Setup

* Install **Yarn** and **Node.js**. See [Guide for NodeJs](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) and [Yarn install](https://classic.yarnpkg.com/lang/en/docs/install)<br/>
*Supported versions:*
```bash
"engines": {
    "node": "^14.17.6",
    "npm": "^6.14.15"
  }
```
* Install [Nx CLI](https://nx.dev/using-nx/nx-cli) globally to enable running **nx executable commands**.
```bash
yarn global add nx
```
* Clone the GitHub repository (`wget` need to be installed first):

```bash
git clone https://github.com/BerithFoundation/Berith-IDE.git
```
* Build `berith-ide-project`:
```bash
cd berith-ide-project
yarn install
yarn run build:libs // Build berith-ide libs
nx build
nx serve
```

Open `http://127.0.0.1:8080` in your browser to load Berith IDE locally.

Go to your `text editor` and start developing. The browser will automatically refresh when files are saved.

## Production Build
To generate react production builds for berith-ide-project.
```bash
yarn run build:production
```
Build can be found in `berith-ide-project/dist/apps/remix-ide` directory.

```bash
yarn run serve:production
```
Production build will be served by default to `http://localhost:8080/` or `http://127.0.0.1:8080/`

