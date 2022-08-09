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