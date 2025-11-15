Severance v5 iOS Project - Build Instructions

This package contains the web app in `www/` and iOS wrapper sources. To produce a signed .ipa you have two options:

A) Build locally on a Mac with Xcode
   1. Create a new Xcode iOS App project (App template).
   2. Replace AppDelegate.swift, SceneDelegate.swift, ViewController.swift and Info.plist with the files in this package.
   3. Drag the `www` folder into your project (Copy items if needed).
   4. Add Assets.xcassets/AppIcon.appiconset to the project's asset catalog.
   5. Set Bundle Identifier to com.kevin.Severance, set signing Team.
   6. Build & Run on device or Archive -> Export .ipa

B) Use GitHub Actions / macos runner (free)
   1. Create a GitHub repo and push this package.
   2. Create an Xcode project locally (on a Mac) and commit the .xcodeproj into the repo (this workflow currently expects a .xcodeproj).
   3. Trigger the workflow (Actions -> Build iOS IPA) and download the artifact.
   4. Install the resulting .ipa using AltStore on your iPhone.

If you want me to attempt generating a full .xcodeproj automatically, reply 'generate xcodeproj' and I'll try. Note: generated xcodeproj may need small tweaks in Xcode.
