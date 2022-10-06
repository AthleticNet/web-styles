# Athletic Styles
Shared Bootstrap 5 + in-house styles for AthleticNet and anet-angular repos

## Usage of SCSS dependencies
1. `npm install @athletic/web-styles`
2.  - In a Webpack project (like Angular), add `@import "@athletic/web-styles/src/site-dependencies";` to use the SCSS variables and mixins supplied in this package.
    - In Visual Studio, use a relative path to the package in `node_modules/@athletic/web-styles/src/site-dependencies` which could end you up with an import like `@import "../../node_modules/@athletic/web-styles/src/site-dependencies";`

## Usage of compiled styles
1. `npm install @athletic/web-styles`
2. Use `@athletic/web-styles/dist/Athletic.min.css`

## Updating

1. Make changes, run `npm run build`, compare the diffs in the outputted css, then commit
2. Run `npm run patch` (this will bump from 8.0.2 to 8.0.3 for example and then commit the changes), and push changes to GitHub which will automatically fire off an NPM publish

## To Discuss
- Do we want to authorize Gitpod w/ AthleticNet organization if wanting to do easy devving via Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/AthleticNet/web-styles)
