

## Prerequisites:

NPM:

```shell
brew install node@18
```

YARN

```shell
npm install --global yarn
```

Create App

```shell
npx @backstage/create-app
```

Test the app

```shell
cd poc-backstage
yarn dev
```

Install additional plugins

```shell
yarn workspace app add @backstage/plugin-circleci

```