# ResolveCommonAndroidStudioIssues


# Issue 1: Incompatible Android Gradle Plugin (AGP) Version

The project is using an incompatible version (**AGP 8.3.0**) of the Android Gradle Plugin.  The latest supported version is **AGP 8.2.1**.

## Resolution Options

### Option 1: Modify AGP Version
If you want to continue using your current Android Studio version, you can downgrade the AGP to a supported version.

**Steps:**
1. Open your `build.gradle` file and locate:
   ```kotlin
   plugins {
       id(libs.plugins.android.application)
   }
2. CMD + Click -> Takes you to libs.version.toml
3. Find the **agp** version at the top
4. Modify version to **AGP 8.2.1** (based on what ever the Latest supported version is in the error message)
5. Sync Project

### Option 2: Upgrade android studio
