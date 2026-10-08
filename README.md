# 2048 Redux - Aurum Edition

A mobile 2048 puzzle game with persistent progression, daily challenges, missions, achievements, unlockable themes, and an illustrated foundry setting. Core play works offline. Optional network features include Google AdMob advertising, Google Play purchases, and Google Play Games leaderboards and achievements.

## Android release

- Package: `com.aurum.edition2048`
- Current release: **1.2.0 (18)**
- Minimum Android SDK: **24** (Android 7.0)
- Target Android SDK: **36**
- Contains ads and optional in-app purchases.

## Privacy policy files

- `privacy.html`: complete standalone policy for public web hosting.
- `index.html`: the same policy at the site's root.
- `privacy.txt`: plain-text copy for reviewing and copying.
- `.nojekyll`: keeps GitHub Pages from processing the static files with Jekyll.

The policy is based on the Android app's current local storage, consent, ad, purchase, sharing, and Google Play Games code. It identifies the app and uses the publisher's Google Play App support email as its privacy contact. Keep that store contact accurate and accessible; a direct support email can also be added to the policy. No business name or email address has been invented.

## Fix the missing Google Play privacy page

The existing URL points to a file in an empty repository:
`https://github.com/ayjays132/2048-Redux-Play-Store/blob/main/privacy`

These files have been prepared locally. They are not live merely because this README exists.

1. Upload this folder's files to the root of the public repository `ayjays132/2048-Redux-Play-Store` on its `main` branch. Include `.nojekyll`; do not upload the game's signing key, passwords, or full workspace.
2. In the repository, open **Settings > Pages**. Under **Build and deployment**, select **Deploy from a branch**, choose **main** and **/(root)**, and save.
3. Wait for the Pages deployment to complete. Open the following intended URL in a signed-out browser and verify that it displays the complete policy:
   `https://ayjays132.github.io/2048-Redux-Play-Store/privacy.html`
4. Only after the page is live, paste that HTTPS URL into Google Play Console's **App content > Privacy policy** field and save. The root URL also displays the policy. Keep the policy public and viewable without a login, download, or visitor editing rights.

Do not submit the intended Pages URL while it still returns a 404. A local file path or ZIP is not the public URL Google Play asks for.

## In-app access

The current signed app already links to its bundled privacy notice from the Foundry Store at `/legal/privacy.html`. This package provides a more detailed Android policy for the public URL. When incorporating this updated policy into a future app build, replace the Android policy content at that existing path and verify that the in-app link opens it offline. Creating this documentation does not alter the already signed version 18 bundle.

## Google Play Data safety notes

Offline saves do not mean the whole app has no data collection. Review the installed SDKs and live AdMob configuration when completing the form.

- **AdMob:** review approximate location inferred from IP, device/account identifiers, ad or app interactions, and diagnostics, including advertising, measurement, analytics, and fraud-prevention purposes. Advertising partner or mediation settings can change the inventory.
- **Google Play Games:** review player identifiers, display names, scores, and achievements when the optional feature is used. Sign-in through a Google account is separate from a publisher-operated game account.
- **Purchases:** the app receives transaction and entitlement information. Google processes payment credentials; the app does not receive full card or bank details. Review purchase history separately from payment credentials.
- **Local profile and progress:** selected avatar images, nicknames, saves, and session statistics are kept on the device by the app. Clear Android app storage to remove all local records. In-game statistics resets do not erase every record.
- **Support and sharing:** disclose the information users choose to send where applicable. Do not promise deletion of Google's records through a local save reset.

The live Data safety declaration must cover all versions and configurations distributed under this package. This README is an inventory to help complete the declaration, not an auto-filled submission or a claim that Google has approved it. Match the target-audience declaration and advertising setup to the audience actually offered the game.

## References

- [Google Play User Data and privacy policy requirements](https://support.google.com/googleplay/android-developer/answer/10144311?hl=en)
- [Google Play Data safety guidance](https://support.google.com/googleplay/android-developer/answer/10787469?hl=en)
- [Google Mobile Ads data disclosures](https://developers.google.com/admob/android/privacy/play-data-disclosure?hl=en) (the current page describes the latest SDK; also verify the SDK version packaged by this app).
- [GitHub Pages publishing-source setup](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

Prepared October 8, 2026. Hosting, Play Console submission, publisher contact details, and provider account configuration remain controlled by the publisher.
