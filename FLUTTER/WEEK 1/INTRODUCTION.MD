# FLUTTER

## WEEK 1

### WHAT IS FLUTTER?

Flutter is a mobile User Interface framework for creating [native apps](https://searchsoftwarequality.techtarget.com/definition/native-application-native-app#:~:text=A%20native%20application%20is%20a%20software%20program%20that,the%20ability%20to%20use%20device-specific%20hardware%20and%20software.) for IOS and Android. It uses single code-base i.e we will have to write the code for the application only once and the same can run in both the predominant mobile operating systems. The applications created get access to the platform APIs like camera, microphone, etc.

* The single code-base is created using programming language *Dart*.

* Gives a smooth and quick experience when running apps.

* Works well with [Firebase](https://howtofirebase.com/what-is-firebase-fcb8614ba442) as a backend.

### PREREQUISITES

* A good understanding on programming concepts.
  * Classes
  * Functions and methods
  * Variables
 
### INSTALLATION

Flutter can be used in any of the editors like *Android Studio or VS code*, in this course I will be using Android Studio but if you prefer to use VS code then refer to [this](https://www.c-sharpcorner.com/blogs/create-a-first-flutter-app-in-visual-studio-code).

1. Download Android Studio from [here](https://developer.android.com/studio).

1. Download Git from [here](https://git-scm.com/downloads) according to your system's operating system and install it.
   * Git is a version control system and is used for tracking changes in our code. 

1. Download Flutter for [here](https://flutter.dev/docs/get-started/install) according to your system's operating system.

1. Installation of Flutter SDK-
   * Do not install Flutter in a directory like `C:\Program Files` because it requires elevated privileges. 
   * Instead we can create a folder called src in the C drive and install Flutter in it.
   * To clone the git, open *cmd*.
   * If your cmd's path looks similar to the one below.
   ```
   C:\Users\Name
   ```
   * Then type `cd..` and press enter.
   * Do the above step once again.
   * You will be left with `C:` as your path.
   * Type `cd src` and press enter to go to that folder.
   * To clone git, type the below line and press enter.
   ```
   git clone -b stable https://github.com/flutter/flutter.git
   ```
   * After the cloning is done, go to folder *src* > Flutter > *Flutter console* > type `flutter doctor` and press enter to verify whether flutter is working or not.
     * The Flutter console can be used for running Flutter commands.
   * If you get a green tick then you have installed Flutter correctly. 

   




  
