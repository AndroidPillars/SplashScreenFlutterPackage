# Splash Screen

* A small Splash Screen used for an intro for any flutter application easily using

## For iOS And Android 

* It 's Now Very Simple And Easy To Use 
* Coming Soon Will Add A Greater Functions 
* For Any information Send Message To Me On => monkey4gamesmmm@gmail.com


### ScreenShot
<img src="screenshot.png" height="300et">

## Usage

[Example](https://github.com/KarimMohamed2005/SplashScreenFlutterPackage/blob/master/example/example.dart)

To use this package :

* add the dependency to your [pubspec.yaml](https://github.com/KarimMohamed2005/SplashScreenFlutterPackage/blob/master/pubspec.yaml) file.

```yaml
  dependencies:
    flutter:
      sdk: flutter
    splashscreen:
```

### How to use


``` dart
      new SplashScreen(
      seconds: 14,
      navigate: new AfterSplash(),
      title: new Text('Welcome In SplashScreen'),
      imageNetwork: 'https://i.imgur.com/TyCSG9A.png',
      loaderColor: Colors.blue,
      backgroundColor: Colors.white,
      styleTextUnderTheLoader: new TextStyle(),
      photoHeight: 110.0,
      photoWidth: 110.0,
      photoRadius: 60.0
    );
```

## Example
```dart

import 'package:flutter/material.dart';
import 'package:splashscreen/splashscreen.dart';
void main(){
  runApp(new MaterialApp(
    home: new MyApp(),
  ));
}


class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => new _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return new SplashScreen(
      seconds: 14,
      navigate: new AfterSplash(),
      title: new Text('Welcome In SplashScreen',
      style: new TextStyle(
        fontWeight: FontWeight.bold,
        fontSize: 20.0
      ),),
      imageNetwork: 'https://i.imgur.com/TyCSG9A.png',
      photoHeight: 110.0,
      photoWidth: 110.0,
      loaderColor: Colors.blue,
      backgroundColor: Colors.white,
      styleTextUnderTheLoader: new TextStyle(),
      photoRadius: 60.0,
    );
  }
}

class AfterSplash extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
      title: new Text("Welcome In SplashScreen Package")
      ),
      body: new Center(
        child: new Text("Succeeded!",
        style: new TextStyle(
          fontWeight: FontWeight.bold,
          fontSize: 30.0
        ),),

      ),
    );
  }
}

<<<<<<< HEAD

```
=======
```
>>>>>>> 01742679c01464b04bd8c0fafce0da5af02b1082
