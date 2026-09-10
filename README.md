# SignLeaf public pages

Live site: https://arsh1219.github.io/signleaf-pages/

- [Privacy policy](https://arsh1219.github.io/signleaf-pages/privacy.html)
- [Terms of use](https://arsh1219.github.io/signleaf-pages/terms.html)
- [Support](https://arsh1219.github.io/signleaf-pages/support.html)

Support and privacy contact: arshpreet@billionweb.co.

The public repository is https://github.com/Arsh1219/signleaf-pages. GitHub Pages serves the root of its `main` branch over HTTPS. These are static HTML/CSS pages with no custom analytics, external fonts or scripts. `.nojekyll` disables Jekyll processing.

To publish updates, copy only `index.html`, `privacy.html`, `terms.html`, `support.html`, `styles.css`, `.nojekyll` and this README into the public repository, then commit and push its `main` branch. Keep this directory and the public repository in sync. Do not copy the app workspace into the public repository.

App Profile links and paywall legal links use the URLs in `Configuration/Development.xcconfig` and `Configuration/Production.xcconfig`. Optional local overrides must preserve these URLs unless deliberately changing hosting.

Reviewed against the current app on 10 September 2026: `Telemetry.swift`, `PurchaseService.swift`, `InstallationIdentity.swift`, `ProjectStore.swift`, `SaveCoordinator.swift`, `Models.swift`, `ProfileView.swift`, the capture/editor flows and `PrivacyInfo.xcprivacy`. The pages cover local processing and backup exclusion, default-enabled usage/diagnostics, linked identifiers, coarse location, RevenueCat purchases, Apple Ads attribution, deletion, three free document saves, trial/renewal terms and restore limitations. Current pages are in English.

Apple's standard EULA governs the app license; `terms.html` contains supplemental service terms. The eight app metadata JSON files include the three public URLs and localized description footers linking the privacy policy, terms and standard EULA. These local metadata changes still need to be applied in App Store Connect, including the Privacy Policy and Support URL fields. Confirm that the App Privacy answers match the shipped SDK configuration and enabled dashboard integrations.

Remaining privacy review concern: `Telemetry.swift` defaults collection on and grants analytics storage at startup, while `ProfileView.swift` has no collection control. This content update accurately discloses that behavior; it does not implement consent or withdrawal. Resolve the consent/withdrawal flow, or substantiate an applicable lawful exception, before submission under [Apple guideline 5.1.1(ii)](https://developer.apple.com/app-store/review/guidelines/#data-collection-and-storage). An email request does not remotely disable the app's analytics.

Retention is described by purpose and provider rules; this publication does not configure or verify dashboard retention settings. The Crashlytics 90-day period is attributed to Firebase's published policy, not an invented operator setting. Confirm provider agreements, retention settings and the support mailbox's ability to handle requests before submission. The operator remains identified through the supplied contact without inventing a company, postal address or jurisdiction.

Sources checked: [Apple guidelines 1.5, 2.1, 3.1.2 and 5.1.1](https://developer.apple.com/app-store/review/guidelines/), [App Privacy details](https://developer.apple.com/app-store/app-privacy-details/), [standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), [subscription presentation](https://developer.apple.com/app-store/subscriptions/), [Firebase privacy](https://firebase.google.com/support/privacy), [Analytics regional IP handling](https://support.google.com/analytics/answer/12017362), [Analytics IP handling outside the EU, Switzerland and UK](https://support.google.com/analytics/answer/16871531), [Analytics retention](https://support.google.com/analytics/answer/7667196), [RevenueCat privacy](https://www.revenuecat.com/privacy), and [RevenueCat Apple Ads attribution](https://www.revenuecat.com/docs/integrations/attribution/apple-search-ads).
