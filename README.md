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
