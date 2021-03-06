## Introduction

This is the scaffold of a react application project with express on the server side.

## Getting Started

Clone the repo:
```sh
git clone git@10.214.168.204:full-stack/react-express-scaffold.git
cd app-name
```

Install yarn:
```js
npm install -g yarn
```

Install dependencies:
```sh
yarn global add create-react-app

yarn
```

Start server:
```sh
# Start server
yarn start

# Selectively set DEBUG env var to get logs
yarn start:debug
```


Tests:
```sh
# Run tests written in ES6 
yarn test

# Run test along with code coverage
yarn test:coverage

# Run tests on file change
yarn test:watch

# Run tests enforcing code coverage (configured via .istanbul.yml)
yarn test:check-coverage
```

Lint:
```sh
# Lint code with ESLint
yarn lint

# Run lint on any file change
yarn lint:watch
```

Other gulp tasks:
```sh
# Wipe out dist and coverage directory
gulp clean

# Default task: Wipes out dist and coverage directory. Compiles using babel.
gulp
```

##### Deployment

```sh
# compile to ES5
1. yarn build

# upload dist/ to your server
2. scp -rp dist/* user@dest_ip:/appName

# install production dependencies only
3. yarn --production

# Use any process manager to start your services
4. pm2 start dest_ip/appName/pm2.config.js --watch
```
