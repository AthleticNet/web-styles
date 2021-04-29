# Athletic Styles
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/AthleticNet/web-styles)

Use Athletic7.3.scss in a package for usage on AthleticNet and anet-angular repos
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

## Usage
- In a Webpack project (like Angular), you can then add `@import "~@athleticnet/web-styles/7.3/site-dependencies.scss";` to use the SCSS variables and mixins supplied in this package.
- In Visual Studio, you can then switch from the Shared/styles folder to the package in node_modules doing a find replace that keep the same number of "../": 
`@import "../../Shared/styles/Athletic7.3/site-dependencies";`
`@import "../../node_modules/@athleticnet/web-styles/7.3/site-dependencies";` 

Currently $test-red and $test-blue are variables available for testing

## TODO 
- move all styles into web-styles repo and then update paths to Athletic[6-7].3.css and site-dependences from Visual Studio

### Possible solutions to sharing styles across repos
1. Publish to NPM would make for easier package install, but that makes it harder to publish as each package editor must be authenticated with NPMJS.org (would require making a team organization...). 
2. GitHub packages requires a 1-time authentication with the Github package registry per user, but makes the automatic publish easier as anyone with access to the AthleticNet org can publish by simply creating a new release on GitHub.
3. Continue installing repositories side-by-side, but that leaves our issue of automatic deployments via GitHub actions unsolved