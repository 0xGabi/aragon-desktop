# Aragon Desktop <img align="right" src="https://github.com/aragon/design/blob/master/readme-logo.png" height="80px" />

Aragon Desktop is an Electron app that runs the Aragon client in a fully decentralized way.

It queries the Ethereum blockchain for the latest version of the app, and then serves it over a local IPFS node.

![Screenshot](.github/screenshot.png)

## Running locally

Requires Node v10.x.

```sh
git clone git@github.com:aragon/aragon-desktop
npm i
npm start
```

## Content

When the content `ipfs-hash` of the assets folder change is important to propagate this throgh IPFS. The best way to do this is use the araognCLI command `ipfs propagate`:

```sh
aragon ipfs propagate <ipfs-hash>
```
