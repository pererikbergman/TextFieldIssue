# Text Input Field Issue

This repository demonstrates an issue with text input fields in KMP iOS. Below is a video demonstration of the problem:

https://user-images.githubusercontent.com/pererikbergman/TextFieldIssue/main/mtrl/textinputfield.mp4

## Attempted Solution

We attempted to fix the text input field issue by updating to newer versions of the Kotlin Multiplatform and Compose dependencies. The following changes were made:

1. Updated Kotlin to version `2.1.20-RC2` (from `2.1.0`)
2. Updated Compose Multiplatform to version `1.8.0-alpha03` (from `1.7.0`)
3. Updated Android SDK targets:
   - compileSdk: 35 (from 34)
   - targetSdk: 35 (from 34)
4. Added the JetBrains Compose Maven repository to access the newer versions:
   ```kotlin
   repositories {
       maven("https://maven.pkg.jetbrains.space/public/p/compose/dev")
       // other repositories...
   }
   ```

**Note:** Despite these updates, the text input field issue in the iOS implementation persists. We're continuing to investigate a proper solution.

## Current Status

The issue with text input fields in the iOS implementation remains unresolved. The problem appears to be related to how Compose Multiplatform handles text input on iOS platforms, particularly with focus management and keyboard interactions.

Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)…