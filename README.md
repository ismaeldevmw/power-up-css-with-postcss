# Power-up CSS with PostCSS
PostCSS is an absolutely amazing tool, this is a template with a basic configuration.

To start the project, you must run the next command in your terminal:

```powershell
npm run postcss:watch
```

If you want start from scratch, you can use this command to start.

```powershell
npm init -y
npm i -D postcss postcss-cli
npm i -D postcss-import
npm i -D cssnano postcss-preset-env
```
After that, we add the following configuration on postcss.config.js to start using our plugins.

``` javascript
module.exports = {
  plugins: [
    require('postcss-import'),
    require('postcss-preset-env')({ stage: 1 }),
    require('cssnano'),
  ]
}
```
