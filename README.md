# Flutter Login Example

This example uses a ScrollView, JSON Rest API, Navigation, Alert Pop Up, Progress Indicator, Globals, Images in a shared asset folder, and 100% Shared Code. Now with the ability to login with FaceID, TouchID, and Fingerprint Reader on Android. 

## Getting Started

Clone or Fork Project to get started.

### Prerequisites

Flutter SDK, Android Studio or Other Compatible IDE.

### Demo
<p align="center">
<!--  <img src="https://appleeducate.github.io/flutter_login/screenshots/ezgif.com-video-to-gif.gif" width="450"/> -->
 <img src="https://github.com/AppleEducate/flutter_login/blob/master/screenshots/ezgif.com-video-to-gif.gif" width="350"/>
</p>

#### iOS Integration

Note that this plugin works with both TouchID and FaceID. However, to use the latter,
you need to also add:

```
<key>NSFaceIDUsageDescription</key>
<string>Why is my app authenticating using face id?</string>
```

to your Info.plist file. Failure to do so results in a dialog that tells the user your
app has not been updated to use TouchID.


#### Android Integration

Update your project's `AndroidManifest.xml` file to include the
`USE_FINGERPRINT` permissions:

```
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
          package="com.example.app">
  <uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<manifest>
```

#### Sticky Auth

You can set the `stickyAuth` option on the plugin to true so that plugin does not
return failure if the app is put to background by the system. This might happen
if the user receives a phone call before they get a chance to authenticate. With
`stickyAuth` set to false, this would result in plugin returning failure result
to the Dart app. If set to true, the plugin will retry authenticating when the
app resumes.

## Screenshots
<p align="center"> 
  <img src="https://appleeducate.github.io/flutter_login/screenshots/IMG_0004.PNG" width="350"/>
  <img src="https://appleeducate.github.io/flutter_login/screenshots/Screenshot_20180411-133707.png"  width="350"/>
</p>

### Fingerprint Reader and TouchID/FaceID
<p align="center">
  <img src="https://appleeducate.github.io/flutter_login/screenshots/IMG_1413.jpg" width="350"/>
  <img src="https://appleeducate.github.io/flutter_login/screenshots/Screenshot_20180411-133646.png" width="350"/>
</p>

## Built With

* [Flutter](https://flutter.io) - Crossplatform App Development Framework

## Contributing
Please submit a pull request if you want to help the project grow. The goal is to be able to fork the project and have a login module for your app complete so that a new project can be started quickly and customized to the user's needs.

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Rody Davis** - *Initial work* - [Rody Davis](https://github.com/AppleEducate)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* https://flutter.io/networking/
* https://github.com/bramvbilsen/Flutter-HTTP-Requests-REST-api
* https://github.com/Solido/awesome-flutter
* https://reqres.in
* https://github.com/GeekyAnts/FlatApp-Flutter
