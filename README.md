# Expo CLI: Resolving Native Module Linking Errors

This repository demonstrates a common issue in Expo projects where updating the Expo CLI or SDK version leads to native module linking errors during the build process for iOS or Android.  The problem arises from a mismatch between the native module versions and the updated Expo SDK.

## Problem Description

After updating Expo CLI or SDK, you might encounter linking errors.  These errors typically occur during the build process and can manifest as linker errors, missing header files, or similar compilation issues related to the native modules within your project's `ios` and `android` folders.

## Solution

The solution involves ensuring that the native modules are synchronized with the current Expo SDK version.  This usually involves cleaning the build cache, and in some cases, re-linking native dependencies using the expo prebuild command.

## Reproduction Steps (For `expoBug.js`)

1.  Update Expo CLI to a newer version
2.  Update the Expo SDK version in your `app.json`
3.  Attempt to run the project with `expo start`.

## Code Example (`expoBug.js`):

This example is not needed for reproducing the error, as the problem occurs in the native module linking step and does not usually stem from Javascript code.