# flutter-clean-archi-model
Flutter app built with clean archi + technical doc

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## FVM

FVM is a must have tool for managing Flutter SDK versions and is used in this project.
Check out the [FVM documentation](https://fvm.app/documentation/getting-started) for more details.

### Installation

Install fvm via Homebrew (macOS) 
```brew tap leoafarias/fvm && brew install fvm```

### Install and use the project flutter version

Install a specific Flutter version :   
```fvm install <version> ```  
Ex : `fvm install 3.35.7`

Use the version specified in the project (in file `.fvm`) : 
```fvm use```

Change version specified in the project (file `.fvm` will be edited) :  
```fvm use <version>```

Use FVM to execute Flutter commands :
```fvm flutter pub get```  
```fvm flutter run```

### Android Studio configuration

1. Open `Settings` > `Languages & Frameworks` > `Flutter`
2. For the *Flutter SDK* path field, point to the SDK managed by FVM in the project: `./.fvm/flutter_sdk` (an absolute path from the project root is recommended).
    - Exemple : `/Users/<username>/path/to/project/.fvm/flutter_sdk`
3. Restart Android Studio if necessary so the plugins detect the new SDK.
4. In Android Studio's integrated terminal, use `fvm flutter <command>` or set up an alias so actions use the FVM-managed Flutter version.
5. For CI or scripts, export `FLUTTER_ROOT` to `./.fvm/flutter_sdk` or explicitly use `fvm` in your pipelines.
