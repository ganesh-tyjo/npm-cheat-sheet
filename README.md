<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<br />
<p align="center">
<a href="https://npmjs.com">
    <img src="./content/images/npm-logo.png" alt="NPM" height="50" width="auto" >
  </a>
<p align="center"><strong>NPM Cheat Sheet</strong></p>
</p>

---

<br />
<details open="open">
  <summary><strong>Table of Contents</strong></summary>

- [Get Version](#get-version)
- [Get Help](#get-help)
- [Create package.json](#create-packagejson)
- [Set Defaults](#set-defaults)
- [Get Defaults](#get-defaults)
- [Remove Defaults](#remove-defaults)
- [Install Packages](#install-packages)
- [Install Certain Version](#install-certain-version)
- [Update Packages](#update-packages)
- [Remove Packages](#remove-packages)
- [Move to Another Folder](#move-to-another-folder)
- [Find Root Folder](#find-root-folder)
- [List Packages](#list-packages)
- [NPM Scripts](#npm-scripts)
- [Package Version](#package-version)

</details>

## Get Version

```bash
npm -v

npm --version
```

## Get Help

```bash
npm

npm help
```

## Create package.json

```bash
npm init

npm init -y

npm init --yes
```

## Set Defaults

```bash
npm config set init-author-name 'YOUR NAME'

npm config set init-license 'MIT'
```

## Get Defaults

```bash
npm config get init-author-name

npm config get init-license
```

## Remove Defaults

```bash
npm config delete init-author-name

npm config delete init-license
```

## Install Packages

Globally

```bash
npm install -g package-name
```

Production dependency

```bash
npm install --save package-name
```

Development dependency

```bash
npm install --save-dev package-name
```

## Install Certain Version

Globally

```bash
npm install -g package-name@package-version
```

Production dependency

```bash
npm install --save package-name@package-version
```

Development dependency

```bash
npm install --save-dev package-name@package-version
```

## Update Packages

Globally

```bash
npm update -g package-name
```

Production dependency

```bash
npm update --save package-name
```

Development dependency

```bash
npm update --save-dev package-name
```

## Remove Packages

Globally

```bash
npm uninstall -g package-name
```

Production dependency

```bash
npm uninstall --save package-name
```

Development dependency

```bash
npm uninstall --save-dev package-name
```

## Move to Another Folder

Install production and development dependencies.

```bash
npm install
```

Install production dependencies only.

```bash
npm install --production
```

## Find Root Folder

Globally

```bash
npm root -g
```

Locally

```bash
npm root
```

## List Packages

Globally

```bash
npm list -g

npm list -g --depth 0

npm list -g --depth 1
```

Locally

```bash
npm list

npm list --depth 0

npm list --depth 1
```

## NPM Scripts

Define scripts in `package.json` file.

```javascript
"scripts": {
  "start": "node index.js",
  "script-name":"command-to-run"
}
```

Run scripts

```bash
npm start

npm run script-name
```

## Package Version

Find below, What package version with different symbols (\*, ~, ^) represents in `package.json` file.

| Version         | Result                                                                   |
| --------------- | ------------------------------------------------------------------------ |
| "\*"            | Install package with latest version                                      |
| "4.17.3"        | Install package with exact version                                       |
| "~4.17.**`3`**" | Install package with latest patch update (Highlighted part gets updated) |
| "^4.**`17.3`**" | Install package with latest minor update (Highlighted part gets updated) |

Most Preferred

```javascript
"package-name": "^4.17.3"
```

<!-- MARKDOWN LINKS & IMAGES -->

[contributors-shield]: https://img.shields.io/github/contributors/ganesh-tyjo/npm-cheat-sheet.svg?style=for-the-badge
[contributors-url]: https://github.com/ganesh-tyjo/npm-cheat-sheet/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/ganesh-tyjo/npm-cheat-sheet.svg?style=for-the-badge
[forks-url]: https://github.com/ganesh-tyjo/npm-cheat-sheet/network/members
[stars-shield]: https://img.shields.io/github/stars/ganesh-tyjo/npm-cheat-sheet.svg?style=for-the-badge
[stars-url]: https://github.com/ganesh-tyjo/npm-cheat-sheet/stargazers
[issues-shield]: https://img.shields.io/github/issues/ganesh-tyjo/npm-cheat-sheet.svg?style=for-the-badge
[issues-url]: https://github.com/ganesh-tyjo/npm-cheat-sheet/issues
[license-shield]: https://img.shields.io/github/license/ganesh-tyjo/npm-cheat-sheet.svg?style=for-the-badge
[license-url]: https://github.com/ganesh-tyjo/npm-cheat-sheet/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/ganesh-tyjo
