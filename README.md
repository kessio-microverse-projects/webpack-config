# webpack-config
> Webpack is used to compile JavaScript modules. Once installed, you can interact with webpack either from its CLI or API. 

# Getting Started with WebPack

### Step - 1

#### Basic Setup
-  First initialize npm, install webpack locally, and install the webpack-cli (the tool used to run webpack on the command line)

```
npm install webpack webpack-cli --save-dev
```

## Step -2 
- Adjust package.json file in order to make sure we mark our package as private, as well as removing the main entry. - This is to prevent an accidental publish of code. 

## Step - 3
- Now we'll create directory with files and their contents

## Step - 4 

#### Creating a Bundle
> First we'll tweak our directory structure slightly, by creating a dist folder where we'll put the index.html
- Bundle the lodash dependency with index.js, we'll need to install the library locally.
- When installing a package that will be bundled into your production bundle, you should use npm install --save. If you're installing a package for development purposes (e.g. a linter, testing libraries, etc.) then you should use npm install --save-dev

##### Import lodash
> Now, since we'll be bundling our scripts, we have to update our index.html file. Let's remove the lodash <script>, as we now import it, and modify the other <script> tag to load the bundle, instead of the raw ./src file:
 
 ```
 npm install --save lodash
 ```

## Step - 5

#### Run WebPack
>  let's run npx webpack, which will take our script at src/index.js as the entry point, and will generate dist/main.js as the output. The npx command, which ships with Node 8.2/npm 5.2.0 or higher, runs the webpack binary (./node_modules/.bin/webpack) of the webpack package we installed in the beginning.
- Open index.html from the dist directory in your browser and, if everything went right, you should see the following text: 'Hello webpack'.

```
 npx webpack
```

## Step - 6
 #### Using a Configuration

 > As of version 4, webpack doesn't require any configuration, but most projects will need a more complex setup, which is why webpack supports a configuration file. This is much more efficient than having to manually type in a lot of commands in the terminal, so let's create one.
 - Run the build again but instead using our new configuration file:

 ```
 npx webpack --config webpack.config.js
 ```
 - A configuration file allows far more flexibility than CLI usage. We can specify loader rules, plugins, resolve options and many other enhancements this way.
