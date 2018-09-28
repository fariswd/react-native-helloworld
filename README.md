# Native Module: react-native-helloworld
Getting started to write React Native bridge module for Android.

## How to Use the Module
1. Create a new React Native project:

    ```bash
    react-native init NewProject
    ```
2. Add the local module to dependencies in **package.json**: 

    ```js
    "dependencies": {
		...
		"react-native-helloworld":"git+https://github.com/fariswd/react-native-helloworld.git"
	},
    ```
3. Link dependencies:

    ```bash
    react-native link
    ```
4. Use the module in **index.android.js**:

    ```javascript
    import MyModule from 'react-native-helloworld';

    const onButtonPress = () => {
        MyModule.alert('Hello World');
    };
    ```
    
## Blog
[React Native Bridging Modules for Android from Scratch on Windows][1]

[1]:http://www.codepool.biz/react-native-bridging-modules-android.html
