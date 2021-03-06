
# NODEJS

## BASIC

- https://github.com/i0natan/nodebestpractices
- https://github.com/microsoft/nodejs-guidelines
- https://github.com/goldbergyoni/nodebestpractices
- https://github.com/lirantal/nodejs-cli-apps-best-practices
- https://nodesource.com/blog/nine-fantastic-utilities-for-the-node-js-developer
- https://blog.bitsrc.io/npm-tips-and-tricks-24c5e9defea6
- https://nemethgergely.com/nodejs-best-practices-how-to-become-a-better-developer-in-2018/

## NVM

- https://github.com/coreybutler/nvm-windows
- https://github.com/nvm-sh/nvm
- https://github.com/pnpm/pnpm
- https://github.com/tj/n

## LIST
- https://github.com/lirantal/awesome-nodejs-security
- https://github.com/parro-it/awesome-micro-npm-packages
- https://dev.to/madza/73-awesome-npm-packages-for-productivity-19p8
- https://www.prisma.io/dataguide/database-tools/top-nodejs-orms-query-builders-and-database-libraries-in-2020

## UTILS

- https://github.com/radarsu/types-package-json
- https://github.com/davglass/license-checker
- https://github.com/localtunnel/localtunnel
- https://github.com/sindresorhus/fkill-cli
- https://github.com/juliangruber/npm-diff
- https://github.com/SBoudrias/Inquirer.js
- https://github.com/folke/ultra-runner
- https://github.com/voidcosmos/npkill
- https://github.com/depcheck/depcheck
- https://github.com/sindresorhus/np
- https://github.com/typicode/husky
- https://github.com/ranyitz/newsh
- https://github.com/lirantal/npq
- https://github.com/amio/npm-why
- https://github.com/ranyitz/qnm
- https://github.com/vercel/ncc
- https://github.com/vercel/nft
- https://github.com/sezna/nps

## MONITORING

- https://clinicjs.org/
- http://pm2.keymetrics.io/

## LIBS

- https://github.com/azz/pretty-quick
- https://github.com/clinicjs/node-clinic
- https://github.com/theophilusx/ssh2-sftp-client
- https://github.com/panva/node-oidc-provider
- https://github.com/microsoft/playwright
- https://github.com/arcanis/clipanion
- https://github.com/sindresorhus/got
- https://github.com/expressjs/multer
- https://github.com/verdaccio/verdaccio
- https://github.com/mcollina/on-exit-leak-free
- https://github.com/Unitech/pm2

## SERVER: EXPRESS/ITTY
- https://github.com/YahooArchive/express-state
- https://github.com/mucahitnezir/express-starter
- https://github.com/kwhitley/itty-router-extras
- https://github.com/kwhitley/itty-router

## FRAMEWORKS

- https://github.com/nestjs/nest
- https://github.com/strapi/strapi
- https://github.com/lukeautry/tsoa
- https://github.com/typeorm/typeorm
- https://github.com/directus/directus
- https://github.com/mikro-orm/mikro-orm
- https://github.com/sequelize/sequelize
- https://github.com/strongloop/loopback-next

## CLI

- https://docs.npmjs.com/cli/ci.html
- https://michael-kuehnel.de/tooling/2018/03/22/helpers-and-tips-for-npm-run-scripts.html


## NODE UPDATE WINDOWS

1. download & install node : latest version from official website
2. use npm-windows-upgrade to update npm

## COMMANDS


## NPM

### Helper

```
npm list -g --depth 0 (list the global package installed)
npx ... (run directly a global or local package from the node_modules)
npx ngcc (example to run angular ngcc in an angular (v9) project)
```

### Versions

- package version has 3 parts - major.minor.patch
- ^ = latest minor version will be installed
- ~ = latest patch version will be installed

```
rm -rf package-lock.json
rm -rf node_modules
npm outdated # check the dep to update
npm update # update all to the wanted
npm update mypackage1 # update one to the wanted
npm update mypackage1 mypackage2 # update many to the wanted
npm install mypackage1@latest # update one to the latest (major)
npx npm-check-updates -u # update all to the latest (major)
```