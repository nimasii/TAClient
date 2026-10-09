# UI review preview

`UIReviewPreview` is a simulator-only companion target for reviewing the redesigned screens with synthetic data. It reuses the production SwiftUI screens and navigation while injecting in-memory repositories and a fresh, isolated preferences suite. It does not load saved credentials, contact a server, or write to the production archive.

The preview replaces remote artwork with local placeholders and replaces the player area with an explicit preview card. Playback and the MobileVLCKit package are not part of this target; the production target and player code remain unchanged.

Open `UIReviewPreview.xcodeproj`, select the `UIReviewPreview` scheme, and run it in an iOS Simulator. The scheme supports iOS Simulator only and disables code signing. Use the `Preview appearance` control in the navigation bar to review System, Light, and Dark appearance.

The simulator captures in `review-artifacts/runtime-screenshots/` document the library, detail, settings, playlists, download queue, and empty download states.
