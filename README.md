# VSCode Android Port

This is an open-source port of Visual Studio Code (VSCode) for Android, providing a fully functional development environment on your mobile device. With this app, you can log in, use remote repositories, SSH, install extensions, run code, and more—all on Android!

## Features

- **Login & Authentication**: Log into your GitHub or other remote repositories.
- **Remote Repositories**: Clone, push, and pull from Git repositories.
- **SSH**: Use SSH to access remote servers directly from the app.
- **Extensions**: Install and manage VSCode extensions.
- **Run Code**: Execute your code right on your Android device, with full support for languages like Python, JavaScript, and more.
- **Full VSCode Functionality**: Almost all VSCode features are ported over, so you can work just as you would on a desktop!

## How to Build and Install the App

Follow these steps to quickly build and install the app on your Android device. I've included simple copy-paste commands for **Debug** and **Release** builds.

### Prerequisites
- **Java Development Kit (JDK)** version 8 or above
- **Gradle** (Gradle version 7.x or higher recommended)
- **Android SDK** installed

### 1. **Clone the Repository**:
`git clone https://github.com/Fundiman/VSCodeAndroid.git`
`cd VSCodeAndroid`

### 2. **Install Dependencies** (optional but recommended):
If you haven't already, run this to ensure everything is set up:
`gradle build`

### 3. **Build and Install the APK**:

#### **For Debug Build (Fastest for testing)**:
Just copy-paste the following command to build and install the APK for debugging:
`gradle assembleDebug && adb install app/build/outputs/apk/debug/app-debug.apk`

#### **For Release Build (For final production)**:
If you’re ready for a release build, use this command:
`gradle assembleRelease && adb install app/build/outputs/apk/release/app-release.apk`

### Troubleshooting
- **Build Failures**: If the build fails due to dependencies, ensure that your `gradle.properties` and `build.gradle` files are correct.
- **Device Compatibility**: Make sure your device has enough resources (especially RAM) to run VSCode.

## Contributing

Feel free to fork the repository, make improvements, and submit pull requests. All contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This is an unofficial port of Visual Studio Code for Android. It is not endorsed by or affiliated with Microsoft in any way. The original VSCode app is developed and maintained by Microsoft.
