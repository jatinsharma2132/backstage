# [Backstage](https://backstage.io)

## Backstage - IDP

## Environments you need before start

### Prerequisites
* Node.js [Active LTS Release](https://nodejs.org/en/blog/release/) installed using one of these methods
    * Using [nvm](https://nodejs.org/en/blog/release/) (recommended)
        * [Installing nvm](https://github.com/nvm-sh/nvm#install--update-script)
        * [Install and change Node version with nvm](https://nodejs.org/en/download/package-manager/#nvm)
    * [Binary Download](https://nodejs.org/en/download/)
    * [Package manager](https://nodejs.org/en/download/package-manager/)
    * [Using NodeSource packages](https://github.com/nodesource/distributions/blob/master/README.md)
* yarn [Installation](https://classic.yarnpkg.com/en/docs/install)
* docker [installation](https://docs.docker.com/engine/install/)
* git [installation](https://github.com/git-guides/install-git)


| Name                      | Where to get?                                                                                                   |
| :------------------------ | :-------------------------------------------------------------------------------------------------------------- |
| GITHUB_ACCESS_TOKEN       | Generate a new personal access token in [GIthub Secure page](https://github.com/settings/tokens)                |
| AUTH_GITHUB_CLIENT_ID     | Get in [Github app ID](https://github.com/settings/applications/new)             |
| AUTH_GITHUB_CLIENT_SECRET | Get in the client section  secrets                                               |
| Homepage URL | http://localhost:3000                                   |
| Authorization callback URL | http://localhost:7007/api/auth/github/handler/frame                                   |
| APPLICATION REGISTRATION | ![Screenshot](https://backstage.io/docs/assets/getting-started/gh-oauth.png)                                   |

All environments above `MUST` be exported in your bash context like below:

```sh
# .bashrc or .zshrc
export GITHUB_ACCESS_TOKEN='YOUR-TOKEN-HERE'
export AUTH_GITHUB_CLIENT_ID='YOUR-TOKEN-HERE'
export AUTH_GITHUB_CLIENT_SECRET='YOUR-TOKEN-HERE'
```

### To start the app, run:
Note : The engine "node" is compatible with version "14 || 16".
```sh
nvm install 16        # Install v16
nvm use 16            # Use v16
```
Change to the backstage-app folder and run the following

```sh
yarn install
yarn dev
```
