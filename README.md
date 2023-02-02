# POC Backstage

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

# cp -f files/app-config.yaml backstage/app-config.yaml
patch backstage/app-config.yaml files/app-config.yaml.patch
cp -f files/examples/poc.yaml backstage/examples/poc.yaml
```

Test the app

```shell
yarn --cwd backstage dev
```

## Examples

Install additional plugins
```shell
yarn add --cwd backstage/packages/app @backstage/plugin-api-docs

```
Create the patch
```shell
diff -u backstage/app-config.yaml files/app-config.yaml > files/app-config.yaml.patch
```