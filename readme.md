# Example of browserify bundled local module

This is just a sample of the pieces needed if you wanted to create a commonjs module that uses jquery and handlebars, then bundle this with browserify using hbsfy transform so handlebars templates are precompiled

There is one local module here: node_modules/app-account-settings
It has a a dependency on jquery so if you want to compile this again you would have to perform an npm install inside that module directory for jquery, then perform an npm install at the top level to get handlebars and hbsfy, then you could recreate the output via:

```
browserify main.js > bundle.js
```
