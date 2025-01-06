Command to create the project: `npx create-expo-app tracks --template blank`

Other option to create project: `npx expo-cli init tracks`

Install Below Libraries:

1. Install React Navigation : `npm install react-navigation@4.4.4 --legacy-peer-deps`

2. Install Dependencies

`npx expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view -- --legacy-peer-deps`

3. Install React Navigation Stack

`npm install react-navigation-stack @react-native-community/masked-view --legacy-peer-deps`

4. Install React Navigation Material Bottom Tabs Library:

`npm install react-navigation-material-bottom-tabs react-native-paper@4 --legacy-peer-deps`

5. Create a babel.config.js file at the root of the project (where package.json file is located) and add the following code:

```module.exports = function (api) {
  api.cache(true);
  return {
    presets: ["babel-preset-expo"],
    plugins: ["react-native-reanimated/plugin"],
  };
};