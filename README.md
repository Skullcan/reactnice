<h3 align="center">REACT NICE (0.69.1)</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/skullcan/reactnice.svg)](https://github.com/skullcan/reactnice/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/skullcan/reactnice.svg)](https://github.com/skullcan/reactnice/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> Clean react-native init project with configurations and changes made to succefully build in Windows using the new architecture.
    <br> 
</p>

## 📝 Table of Contents

-   [About](#about)
-   [Getting Started](#getting_started)
-   [Usage](#usage)
-   [Changes made](#changes)
-   [Acknowledgments](#acknowledgement)

## 🤘 About <a name = "about"></a>

The intent is to create a baseline project for others to check if their setup is ready to build the react-native project using the new architecture.

## 🏁 Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

-   Make sure your environment is setup correctly. https://reactnative.dev/docs/environment-setup
-   Verify it using npx @react-native-community/cli doctor (thanks [@truediogo](https://github.com/truediogo))
-   Make sure you have followed the instruction for successfully compiling the bundled Hermes in: https://reactnative.dev/architecture/bundled-hermes#android-users-on-new-architecture
-   Make sure you are using the Visual Studio Developer Command Prompt. https://reactnative.dev/docs/visual-studio-command-prompt.
-   Download and extract the binaries of the ICU4C library. At this moment the latest version is:
https://github.com/unicode-org/icu/releases/tag/release-71-1
-   Add the ICU4C folder to your PATH in the Enviroment Variables. ie: C:\icu4c\bin


## 🎈 Usage <a name="usage"></a>

After you cloned the repository, you can run the project using the following command:

```
yarn install && yarn android
```

## ✅ Changes made <a name = "changes"></a>

You can check all the changes in the [commits](https://github.com/Skullcan/reactnice/commits/master), but most important one is:

-   Added the [import](https://github.com/Skullcan/reactnice/blob/b1accfd5df286fb6b4713d1def7d56ee0fa92760/android/build.gradle#L1) and [IF](https://github.com/Skullcan/reactnice/blob/b1accfd5df286fb6b4713d1def7d56ee0fa92760/android/build.gradle#L15) in the project/build.gradle file for the NDK version 23.1.7779620. This is to prevent the error with long path files during the build process.

## ✍️ Authors <a name = "authors"></a>

-   [@Skullcan](https://github.com/Skullcan)

## 🎉 Acknowledgements <a name = "acknowledgement"></a>

-   [@aleluiah](https://github.com/aleluiah) (OP)
-   [@cortinico](https://github.com/cortinico)
-   [@vikassahu305](https://github.com/vikassahu305)
-   [@truediogo](https://github.com/truediogo)
-   [@JoseLion](https://github.com/JoseLion)

And all the people who commented and tried to help in the issue: [#34084](https://github.com/facebook/react-native/issues/34084)
