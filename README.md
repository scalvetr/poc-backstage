

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

cp -f files/app-config.yaml backstage/app-config.yaml
cp -f files/examples/poc.yaml backstage/examples/poc.yaml
```

Test the app

```shell
cd backstage
yarn dev
```

Install additional plugins

```shell
yarn workspace app add @backstage/plugin-circleci

```