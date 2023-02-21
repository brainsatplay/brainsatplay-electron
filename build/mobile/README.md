# MyAlyce_Dev
 Development Env Repo for MyAlyce

 Install project dependencies by running `npm install` in the root directory.

#### Android

With Android Studio installed:
- `npx cap add android`
- `npx cap copy`
- `npx cap open android`

If you do not have our AndroidManifest.xml in `android/app/src/main`, ensure these permissions are available, placed under the <!-- Permissions --> tag in the file created by capacitor:
```xml
<uses-permission android:name="android.permission.ACCESS_BACKGROUND_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"  />
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"  />
<uses-permission
    android:name="android.permission.BLUETOOTH"
/>
<uses-permission
    android:name="android.permission.BLUETOOTH_ADMIN"
/>
<uses-permission
    android:name="android.permission.BLUETOOTH_SCAN"
    tools:targetApi="s"
/>
<uses-permission
    android:name="android.permission.BLUETOOTH_CONNECT"
    tools:targetApi="s"
/>

<uses-permission android:name="android.permission.INTERNET" />
```

The first run will likely need to install all of the tools in the android project necessary. Build the android project in Android Studio after running these commands by clicking the Make Project hammer icon if it doesn't start automatically. Then if you see BUILD SUCCESSFUL, run with your android device connected or the built-in android emulators active.

#### IOS 

With XCode installed:
- `npx cap add ios`
- `npx cap copy`
- `npx cap open ios`
