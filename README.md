# legal/

Source for the public privacy policy that the App and the stores link to.

## Hosting

These files are intended to be copied into a separate, public GitHub repository (suggested name: `waveclean-legal`) and served via GitHub Pages.

### Publishing steps

1. Create a new public repo on GitHub: `waveclean-legal`.
2. Copy `index.md` and `privacy.md` into the root of that repo.
3. Commit and push to `main`.
4. In the repo's **Settings → Pages**, set:
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
5. After ~1 minute the policy will be live at:
   `https://codingwithsalman.github.io/waveclean-legal/privacy`
6. Update `PRIVACY_POLICY_URL` in `composeApp/src/commonMain/kotlin/com/cws/waveclean/AppInfo.kt` to that URL and commit.

## Updating

Treat the `legal/` folder in this repo as the source of truth. When the policy changes, update `legal/privacy.md` here, then sync the change into `waveclean-legal` and bump the **Last updated** date inside the file.
