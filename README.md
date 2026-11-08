# Hostel Productivity Predictor (installable app)

Choose your hostel room conditions (room sharing, noise, comfort, Wi-Fi, interruptions) and the app instantly predicts study productivity: **Low, Mid or High**.

It is the final model of the project *Impact of Hostel Environment on Student Study Productivity* (Data Science with AI, NITK): a tuned SVM with test accuracy 0.83 and macro-F1 0.77. The model was run on all 1,250 possible answer combinations, and the app shows those exact predictions. Mid is the model's weakest class. This is a screening tool based on self-reported survey data, not a judgement on any student.

**Made by:** Rishi Yadav (261CS243), Section 14, Computer Science, NITK

## Files
| File | What it is |
|---|---|
| `index.html` | The app (all the code and the model's predictions are inside) |
| `manifest.json` | Tells the phone the app's name, colours and icon |
| `sw.js` | Lets the app open even without internet after the first visit |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | The app icon |

## Put it online so anyone can use it (free, GitHub Pages)
1. On github.com, tap **+ > New repository**. Name it `hostel-productivity-app`, choose **Public**, tick "Add a README" and tap **Create repository**.
2. Tap **Add file > Upload files** and upload all 6 files (`index.html`, `manifest.json`, `sw.js` and the 3 PNG icons). Tap **Commit changes**.
3. Go to **Settings > Pages**. Under "Build and deployment", choose **Deploy from a branch**, select branch `main` and folder `/ (root)`, and tap **Save**.
4. Wait 1 to 2 minutes and refresh. GitHub shows your link: `https://YOUR-USERNAME.github.io/hostel-productivity-app/`

Anyone with this link can open the app. No login and no installation is needed.

## Put the icon on your home screen
- **Android (Chrome):** open the link, tap the **three dots menu > Install app** (or **Add to Home screen**).
- **iPhone (Safari only):** open the link, tap the **Share button > Add to Home Screen > Add**.
- **Laptop (Chrome or Edge):** click the install icon at the right end of the address bar.

The app then opens full screen with its own icon, like any other app.

## Notes
- Use a **public** repo, because GitHub Pages is free only for public repos. This repo holds only the app, so your report and data stay in your private project repo.
- After you change a file, increase the version in `sw.js` (`hostel-v1` to `hostel-v2`) so that phones fetch the new version.
- This is a web app, not an APK or a Play Store app.
