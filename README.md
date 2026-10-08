# 20 Axes: iOS build without a Mac

1. Create a free GitHub account and a new PUBLIC repository (free macOS build minutes).
2. Upload everything in this folder to the repository, including the hidden `.github` folder.
   If the web uploader skips `.github`, use Add file > Create new file, type
   `.github/workflows/ios.yml` as the name, and paste in the file's contents.
3. Open the repository's Actions tab, choose "Build iOS IPA (unsigned)", click Run workflow.
4. Wait about 10 minutes. Open the finished run and download the `App-ipa` artifact (a zip containing App.ipa).
5. On your Windows PC install iTunes (from apple.com, not the Microsoft Store version if Sideloadly asks)
   and Sideloadly (sideloadly.io). Plug in your iPhone and tap Trust.
6. On the iPhone: Settings > Privacy & Security > Developer Mode > On (it restarts).
7. Drag App.ipa into Sideloadly, enter an Apple ID (a spare one is a good idea), press Start.
8. On the iPhone: Settings > General > VPN & Device Management > your Apple ID > Trust.
9. Open the app. With a free Apple ID it expires after 7 days. Re-run Sideloadly to refresh it.

To update the quiz later: replace www/index.html in the repo, run the workflow again, reinstall.
