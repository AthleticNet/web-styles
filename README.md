# Athletic Styles
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/AthleticNet/web-styles)

Shared Bootstrap 4 + in-house styles for AthleticNet and anet-angular repos

## Usage
1. `npm install @athletic/web-styles`
2.  - In a Webpack project (like Angular), you can then add `@import "~@athletic/web-styles/Athletic7.3/site-dependencies.scss";` to use the SCSS variables and mixins supplied in this package.
    - In Visual Studio, you can then switch from the Shared/styles folder to the package in node_modules doing a find replace that keep the same number of "../": 
`@import "../../Shared/styles/Athletic7.3/site-dependencies";`
`@import "../../node_modules/@athletic/web-styles/Athletic7.3/site-dependencies";` 

## TODO 
- update paths to Athletic[6-7].3.css and site-dependences from both repos

## Updating

1. Make changes and commit
2. Run `npm version patch` and commit, this will automatically fire off an NPM publish