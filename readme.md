# Hulan ESLint Config Package

This package contains Hulan's global ESLint Configuration.

## Installation

To use the ESLint configuration, install this package to your project using the following command:

```sh
$ npm install --save-dev @hulanbv/eslint-config
```

Then add the following to your `.eslintrc` file for **React** projects:

```json
{
  "extends": ["react-app", "@hulanbv/eslint-config"]
}
```

## Development Usage

Install the packages using the Node Package Manager.

```sh
$ npm install
```

To use the package during development, create an archive using the pack command and install the packages manually in your project.

```sh
$ npm pack
$ npm install hulanbv-eslint-config-x.y.z.tgz
```

## Creating Releases and Distribution

The package is distributed automatically to the Node Package Registry using GitHub Actions. In order to publish a new version, you'll need to push over your changes to the master branch including a version tag on the commit you'd like to build. Use the following command will do so. When you've pushed a new tag, make sure this tag matches your package's new version. Check the deployments tab on GitHub to follow the publish process.

```sh
$ npm version [<newversion> | major | minor | patch]
$ git push origin <tag_name>
```
