# Basic Netsuite UIF Single Page Application 

Netsuite User Interface Framework (UIF) is a frontend framework that is used as a UI library for Netsuite Single Page Application (SPA), it is similar to React.

This repository is an example of barebone set up for Netsuite SPA using Netsuite's own example [HelloworldJS](https://github.com/oracle-samples/netsuite-suitecloud-samples/tree/main/spa-suiteapp-samples/helloworld-js) as the basis.

The goal was to understand the minimal set up requirement to create a basic SPA without all the bloated dev dependencies such as formatters and linters. 

You can fork/clone/download this repo's project set up to get started on creating Netsuite SPA, this example uses JavaScript and not TypeScript. Although, TypeScript is a required dev dependencies since the UIF is written in TypeScript.

## Important Note

- tsconfig.json - This file is important as it outline how the TypeScript files should be transpiled, the property `"allowJs": true` means you can develop in JavaScript instead of TypeScript. It also outline where the source files along other things.
- gulpfile.mjs - This file is the automation of the build, it will transpile the TypeScript to JavaScript, concatenate files and minify them based on the setting preference set (variable in the same file). The `rollup` package is used to bundle the different files into one and the `terser` is used to minify the file.

