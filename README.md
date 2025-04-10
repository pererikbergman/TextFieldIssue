# Text Input Field Issue - RESOLVED

This repository was created to demonstrate an issue with text input fields in Compose Multiplatform for iOS, specifically with Thai characters. The issue has now been resolved with the latest version updates.

## Issue Description

The original issue affected text input fields in Compose Multiplatform on iOS when using Thai characters. The TextField component had problems properly handling Thai text: "สวัสดีวันนี้มันจันทร์ ทดสอบภาษาไทย ๅฟ่าา็๊๋ษษ".

## Solution

The issue has been resolved by updating to newer versions of the Kotlin Multiplatform and Compose dependencies. The following changes were made:

1. Updated Kotlin to version `2.1.20-RC2` (from `2.1.0`)
2. Updated Compose Multiplatform to version `1.8.0-beta02` (from `1.7.3`)
3. Updated Android SDK targets:
   - compileSdk: 35
   - targetSdk: 35

## Current Status

✅ **RESOLVED**: The text input field issue in the iOS implementation has been fixed with the version updates mentioned above. The TextField now correctly handles Thai characters.

## Test Case

The repository contains a simple test case with an `OutlinedTextField` that can be prefilled with Thai text. The test demonstrates that the issue has been resolved.

Learn more about [Kotlin Multiplatform](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)…