# legal/

Source for the public privacy policy that the App and the stores link to.

## Hosting

The privacy policy is published on the TriCode Studio website and is served at:

`https://www.tricodestudio.com/privacy/waveclean.html`

This URL is wired into `PRIVACY_POLICY_URL` in `composeApp/src/commonMain/kotlin/com/cws/waveclean/AppInfo.kt` and into both store listings (`store-assets/listing/`).

### Publishing steps

1. Render `privacy.md` to the HTML page hosted at the URL above (the site build/CMS handles this).
2. Deploy the site so the updated policy is live before any app release that changes data collection.
3. Confirm the live page matches `legal/privacy.md` and that the in-app **Settings → Privacy Policy** link opens it.

## Updating

Treat the `legal/` folder in this repo as the source of truth. When the policy changes, update `legal/privacy.md` here, bump the **Last updated** date inside the file, then republish the page at the URL above.
