# NPM courses

## What is npm ?
NPM: Package manager. It's a way to share your code with other developers and reuse code from other devs. It's easy to manage versions.

## Help
3 ways to have some help:

```bash
npm help
```

```bash
npm something -h
```

```bash
npm help-search something
```

## Package.json
This file is to manage dependencies
This file is automatically created when you do a `npm init`.
To put yes to all questions, you can do a 
```bash
npm init --yes
```
or 
```bash
npm init -y
```
To add some informations into the `package.json` file, you can do, for example: 
```bash
npm config get init-author-name
```
To remove some information, you can do, for example:
```bash
npm config delete init-license
```

## Install a package locally
To install a package locally:
```bash
npm install something
```
or
```bash
npm i something
```

To install and save a dependency locally:

```bash
npm install something --save
```
or
```bash
npm i something -S
```

To install and save a dev dependency locally:

```bash
npm install something --save-dev
```

or
```bash
npm install something -D
```
## Uninstall a local package

To uninstall a local dependency
```bash
npm uninstall something --save
```

To uninstall a local devDependency
```bash
npm uninstall something --save-dev
```

## Install a global package

To install a global package

```bash
npm i something -g
```

## Listing package

To list your packages:

```bash
npm list
```

To list your global packages:

```bash
npm list --global true --depth 0
```

## npm versioning

`0.0.0` The first number of a package version is the `major` version, this number is incremented if there is a break in older functions (big changes). 
The second one is the `minor` version, it's when new features is added and if it's not breaking existing features. 
The third one is the `patch` version for fixes.

### Install a specific version

To install a specific version of a package: 
```bash
npm i something@x.x.x
```

To install a specific major and minor version with the latest patch version:
```bash
npm i something@x.x
```

To install a specific major version with the latest minor and patch version:
```bash
npm i something@x
```

## Installing from package.json

```bash
npm install
```

or

```bash
npm i
```

`^0.0.0` stay at the major version but take the latest minor and patch version
`~0.0.0` stay at the major and minor version but take the latest patch version
`"*"` take the latest major, minor and patch version

## Updating packages
To update a dependency:
```bash
npm update something --save
```
To update a global dependency:
```bash
npm update -g something
```

To update all dev dependencies:
```bash
npm update --dev --save-dev
```

To update all dependencies
```bash
npm update
```

To update your global npm version to the latest:
```bash
npm i npm@latest -g
```




