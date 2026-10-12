# ROARISE — Official Privacy & Support Pages

Public pages for the ROARISE iOS app (`com.roarise.alarm`).

- **Privacy Policy:** https://zaka23-cyber.github.io/roarise-privacy-policy/
- **Support:** https://zaka23-cyber.github.io/roarise-privacy-policy/support.html
- **Terms of Use:** https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## Publishing with GitHub Pages

In this repository, open **Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save**. Wait for the site to deploy, then verify both public URLs in an incognito browser.

## Pre-release privacy accuracy checklist

This content is a comprehensive **draft based on the known ROARISE BUILD 03B scope**. The final shipping build must be reviewed before declaring Apple/GDPR compliance.

1. Confirm the official **legal publisher/data controller name and appropriate contact details** for the publicly posted policy, in particular for EU users.
2. Confirm that `z68827163@gmail.com` is the intended public ROARISE privacy/support email. Replace it consistently if a different email is preferred.
3. Inspect the final iOS target, linked frameworks, `Info.plist`, and privacy manifests for every SDK and any data transmitted off-device.
4. Confirm whether RevenueCat is actually included; update the conditional subscription descriptions to match the released app's handling of anonymous IDs, purchases and technical metadata.
5. Align the App Store Connect **App Privacy** disclosure (including third-party SDK collection) with the actual submission build. Do not automatically select “Data Not Collected” if any purchase provider transmits data.
6. Add working in-app links to this privacy policy and Apple's Standard EULA, especially from Settings and the subscription paywall.
7. Verify subscription/trial disclosure and prices on the actual paywall; do not advertise an unimplemented trial.
8. Ensure a support request/deletion process exists and that any retained data can be located and addressed appropriately.
9. Confirm App Store Age Rating, permission strings and localization reflect the shipping features and content.
10. Ensure both pages are publicly reachable over HTTPS without authentication before submitting to App Review.

This repository is for **ROARISE only**. It must not be mixed with the ZELGI repositories.


## Agreed release implementation contract — subscription and privacy

The public Privacy Policy was checked and expanded on October 12, 2026 to name RevenueCat data flows. To avoid later rewriting, BUILD 04 and App Store Connect must implement the **same actual data practices**:

- No ROARISE account/login, no user email collection during app use, and no marketing or advertising trackers in the iOS app.
- Use RevenueCat for StoreKit-backed Pro subscriptions with its generated **anonymous App User ID** unless a deliberate product/legal change is approved. Do not send name, email, alarm time, preferences, microphone input or identifiable custom IDs to RevenueCat.
- RevenueCat processes purchase history and entitlement status. The Apple **App Privacy** form must include **Purchases → Purchase History**, with **App Functionality** and **Analytics** as uses, as directed by RevenueCat's own Apple App Privacy guidance. Decide identity-linkage accurately from the actual IDs and SDK integrations.
- If another SDK is installed or a RevenueCat integration is enabled that sends additional data (for example, ad attribution, analytics, device advertising IDs), STOP and reconcile the policy and App Privacy answers before shipping, not afterward.
- Add a working privacy-policy link and standard Apple EULA link in the app's settings and the subscription paywall. Show accurate localized subscription price, period, auto-renewal, Restore Purchases, cancellation and trial disclosures.
- The planned business offer is **one day of free app access followed by a paid subscription**. This is NOT an Apple-supported one-day StoreKit introductory free trial. Apple's current introductory free-trial minimum is **three days**. A one-day app-level access experience must be designed, tested, disclosed accurately, and must not be presented as an Apple-billed one-day subscription trial.
- No release until actual app code, App Store Connect App Privacy, and the published policy agree. Verify with signed physical-device and StoreKit sandbox purchase/restore/cancel scenarios.
- Formal legal publisher/data-controller identity, public contact details and the intended ROARISE support email must be explicitly confirmed by the publisher before App Review.

Official implementation references:
- https://www.revenuecat.com/docs/platform-resources/apple-platform-resources/apple-app-privacy
- https://www.revenuecat.com/privacy
- https://developer.apple.com/help/app-store-connect/manage-app-information/manage-app-privacy
- https://developer.apple.com/help/app-store-connect/reference/pricing-and-availability/in-app-purchase-and-subscriptions-pricing-and-availability/
- https://developer.apple.com/app-store/review/guidelines/
