# Akku Fantasy — Free-to-play Flutter starter

This is a starter prototype for an Android cricket fantasy app. It uses sample players, sample rankings and demo points only.

## Current prototype includes
- Match centre screen
- Select up to 11 sample players
- Demo points balance (no monetary value)
- Sample leaderboard
- Admin panel UI placeholders

## Not yet connected
- Real login/signup or cloud user accounts
- Live cricket scores / licensed cricket data API
- Cloud database and shared leaderboard
- Secure server-side admin authentication
- Production scoring engine and persistent teams

Do not use this prototype for deposits, paid entry, cash prizes or withdrawals. It intentionally has no real-money features.

## Build an APK using only your Android phone

The easiest route is GitHub Actions, which builds the APK in the cloud.

1. Download and extract `akku_fantasy_project.zip` on your phone.
2. In your browser, create a GitHub account if needed, then create a **new public or private repository** named `akku-fantasy`.
3. Upload the files and folders from this project into the repository, keeping the folder structure:
   - `pubspec.yaml`
   - `lib/main.dart`
   - `.github/workflows/build.yml`
   - `README.md`
4. Open the repository's **Actions** tab. If GitHub asks, enable Actions.
5. Choose **Build Akku Fantasy APK** and tap **Run workflow** (or push a commit to trigger it).
6. When the workflow completes successfully, open the run and download the `akku-fantasy-debug-apk` artifact.
7. Extract the downloaded artifact ZIP on your phone and install `app-debug.apk`. Android may ask you to allow installs from that browser/file manager.

## Important
- A debug APK is for testing, not public release.
- Before a real release, configure app signing, privacy policy, security rules, API keys, backend and tests.
- Never put secret API keys in `lib/main.dart` or any public repository.
- Live cricket scores require a data provider and valid API credentials; sample match data is clearly labelled in the app.
