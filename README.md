# HP Feature Tour — interactive prototype

An interactive prototype of the HP App feature tour on the printer page. The tour card docks to the top of the screen as a header, shows the route to each feature (the tab it taps and the scroll to it), spotlights the feature, and explains it in a coachmark.

It includes two ways of spotlighting a feature, so they can be compared:

| Style | What happens |
|---|---|
| **Outline** | A thin line draws around the feature, then the screen dims. |
| **Pop** | The feature lifts toward you with a thin ring around it as the screen dims. About a second faster per tip. |

## Try it

- **Outline:** `https://<your-username>.github.io/<repo-name>/`
- **Pop:** `https://<your-username>.github.io/<repo-name>/?v=pop`

On a laptop, use the **Highlight style** switch in the panel beside the phone to change styles at any time.

### What to try

1. Tap the blue card, or its play button, to start the tour.
2. Tap X in the blue header, or on a tip, to leave at any point. The card remembers where you stopped; tap it to pick up again.
3. On tip 1, tap **Turn On** to switch on Print Anywhere. Tap **Turn Off**, or the switch itself, to switch it off.
4. On tips 2 and 3, tap **Browse** or **Start a card** to open that feature. The step counts as done; tap the back arrow to return to the paused tour.
5. Finish all three tips, then tap **Done**. The tour card moves to the Help tab; the first time, the app shows you where it went.
6. In Help, tap **Feature tour** to take the tour again. Finish it and the card returns to Help; leave early and the card stays on the page.

Use **Restart prototype** (laptop) to start over.

## Test it on a phone

On a phone the prototype fills the screen, with no phone frame or notes panel. Add it to your home screen to open it like an app, without the browser's address bar.

**iPhone (Safari)**
1. Open the Outline or Pop link in **Safari**. Chrome on iPhone can't add it as an app.
2. Tap **Share**, then **Add to Home Screen**, then **Add**.
3. Open it from the new icon: **Tour Outline** or **Tour Pop**.

**Android (Chrome)**
1. Open the Outline or Pop link in **Chrome**.
2. Tap the **⋮** menu, then **Add to Home screen** or **Install app**.
3. Open it from the new icon.

Add both links to get both styles side by side as two icons.

**Tips**
- A home screen app has no reload button. To start over, close the app and open it again.
- After the files are updated, a phone can keep showing the old version for a few minutes. Close and reopen the app to get the latest.

## Files

| File | Purpose |
|---|---|
| `index.html` | The prototype. Everything, including images, is inside this one file. |
| `pop.html` | Older link for the Pop style; forwards to `?v=pop`. |
| `manifest.json` | Lets Android install the Outline style as an app. |
| `manifest-pop.json` | Lets Android install the Pop style as an app. |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Home screen icons. |
| `README.md` | This file. |

## Publish with GitHub Pages

1. Upload all the files above to the top level of the repository (not inside a folder).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`. The address also appears at the top of the Pages settings.

## Notes

- Needs an internet connection the first time it opens, for the Figtree font.
- The app's interface font is Forma DJR UI. It shows on devices that have it installed; everywhere else Figtree stands in.
- This is a design prototype, not production code. Screens and content are placeholders for testing the tour's flow and motion.
