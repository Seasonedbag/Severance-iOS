
Severance iOS Xcode Project (v5 Full)
------------------------------------

This package contains a generated Xcode project and the `www/` web app folder.

To build:
1. Unzip into a folder.
2. Open `Severance.xcodeproj` in Xcode on a Mac.
3. Ensure Signing & Capabilities has your Apple ID team selected.
4. Build -> Archive -> Export iOS App (.ipa) or run on device.

To use with GitHub Actions:
- Commit the entire project contents to the root of your repo.
- The workflow should run xcodebuild against the .xcodeproj.

Bundle ID: com.kevin.Severance
