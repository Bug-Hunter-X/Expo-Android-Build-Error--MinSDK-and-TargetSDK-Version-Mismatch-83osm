# Expo Android Build Error: MinSDK and TargetSDK Version Mismatch

This repository demonstrates a common error encountered when building Android apps using Expo CLI.  The issue arises from conflicts between the `minSdkVersion` and `targetSdkVersion` values in the `android/app/build.gradle` file, leading to build failures.

## Problem

The Expo CLI build process might fail if the `minSdkVersion` and `targetSdkVersion` are incompatible with the dependencies used in your project.  This typically results in errors related to missing libraries or dependency conflicts.

## Solution

The solution involves carefully reviewing and adjusting the `minSdkVersion` and `targetSdkVersion` values in the `android/app/build.gradle` file to ensure compatibility with your project's dependencies. Often, raising `minSdkVersion` to a more recent value can resolve the issue.  Furthermore, making sure all your dependencies are compatible with both versions is crucial. 

## How to reproduce

1. Clone this repository.
2. Run `expo prebuild`.
3. Attempt to build the Android app using `expo build:android`.
4. Observe the build failure.
5. Apply the solution from `build.gradle.solution` to see the fix.

## License

MIT