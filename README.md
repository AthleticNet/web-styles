# web-styles
Test of using Athletic7.3.scss in a package for usage on AthleticNet and anet-angular repos

## Installing

1. Add `@athleticnet:registry=https://npm.pkg.github.com` to the repo's .npmrc file 
2. Run `npm install @athleticnet/web-styles`

*Note: To install a package from GitHub packages you must do a one-time authentication of yourself with GitHub Packages:* 

```
$ npm login --scope=@athleticnet --registry=https://npm.pkg.github.com

> Username: USERNAME
> Password: TOKEN (create a personal access token in https://github.com/settings/tokens using the repo and read:packages scopes)
> Email: PUBLIC-EMAIL-ADDRESS
```
Source: https://docs.github.com/en/packages/guides/configuring-npm-for-use-with-github-packages#authenticating-with-a-personal-access-token

### Alternatives
Could publish to NPM for easier package install, but that makes it harder to publish. GitHub packages makes the automatic publish easier as anyone with access to the AthleticNet org can publish, whereas NPM makes the consumption easier.