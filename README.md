### Installation

> You first need to clone the project on your computer, and to install [Node](https://nodejs.org). This project also uses [nvm](https://github.com/creationix/nvm), and [yarn](https://yarnpkg.com/).

From the command-line:

```sh
cd ~/Development/sites/
git clone git@github.com:afagin/react-d3-charts.git
cd reusable-d3-charts
```

To install our dependencies:

```sh
nvm install
# Then, install all project dependencies.
yarn install
# Optionally, install the git hooks.
./.githooks/deploy
```

### Working on the project

> Everything mentioned in the installation process should already be done.

```sh
# Start the server and the development tools.
yarn run start
# Builds for production
yarn run build
# Rebuild the styles
yarn run css
# Runs tests.
yarn run test
# Runs linting.
yarn run lint
```

## Deploying a new version

### To production (`gh-pages`)

```sh
# From the project's root.
# Make sure your master is up to date.
git fetch --all
git checkout master
git pull
git push origin master
# Then push the new changes
yarn run deploy
```
