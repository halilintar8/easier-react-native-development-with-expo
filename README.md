# easier-react-native-development-with-expo
A memory game created using Expo for React Native.


npm install --unsafe-perm -g expo-cli

expo init MemoryGame
blank
MemoryGame

cd MemoryGame
npm start

cd ..
git clone https://github.com/tutsplus/easier-react-native-development-with-expo.git
cd MemoryGame
cp -r ../easier-react-native-development-with-expo/components/ ./
mv App.js App.js.old
cp ../easier-react-native-development-with-expo/App.js ./
cp ../easier-react-native-development-with-expo/helpers.js ./

Download expo in playstore
apps - expo - clear data in your android mobile phone

mv app.json app.json.old
vi app.json

{
   "expo": {
    "name": "Memory Game",
    "icon": "./assets/icon.png",
    "version": "1.0.0",
    "slug": "MemoryGame",
    "sdkVersion": "32.0.0",
    "ios": {
      "bundleIdentifier": "com.halilintar8.mymg"
    },
    "android": {
      "package": "com.halilintar8.mymg"
    }
   }
}
 

expo build:android

