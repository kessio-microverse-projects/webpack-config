# webpack-config
> Webpack is used to compile JavaScript modules. Once installed, you can interact with webpack either from its CLI or API. 

## Basic Setup
### 1. Step - 1
-  First initialize npm, install webpack locally, and install the webpack-cli (the tool used to run webpack on the command line)

```
npm install webpack webpack-cli --save-dev
```

## 2. Step -2 
- Adjust package.json file in order to make sure we mark our package as private, as well as removing the main entry. - This is to prevent an accidental publish of code. 

## 3. Step - 3
- Now we'll create directory with files and their contents

## 4. Step - 4 

#### Creating a Bundle
> First we'll tweak our directory structure slightly, by creating a dist folder where we'll put the index.html
- Bundle the lodash dependency with index.js, we'll need to install the library locally.
- When installing a package that will be bundled into your production bundle, you should use npm install --save. If you're installing a package for development purposes (e.g. a linter, testing libraries, etc.) then you should use npm install --save-dev
 
 ```
 npm install --save lodash
 ```


## 5. Step - 5
 #### Using a Configuration

 > As of version 4, webpack doesn't require any configuration, but most projects will need a more complex setup, which is why webpack supports a configuration file. This is much more efficient than having to manually type in a lot of commands in the terminal, so let's create one