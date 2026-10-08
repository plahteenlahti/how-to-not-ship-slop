# Presentations

This repository is the home for Perttu Lähteenlahti's conference presentations.

Open [`index.html`](./index.html) to browse the talks, or open a presentation's
own `index.html` directly to present it in a browser.

## Structure

```text
presentations/
  <talk-slug>/
    index.html          Browser deck
    assets/             Talk-specific images and media
    source/             Source material supplied for the talk
    presentation.pptx   Editable PowerPoint export, when available
```

Each browser deck is self-contained and uses relative asset paths, so it works
from a static file server as well as from the filesystem.

## Deploying on Vercel

This repository is configured as a static Vercel monorepo. Use one Vercel
project for the presentation library and one project for each talk that needs
its own subdomain. Every project connects to this same Git repository.

| Vercel project | Root Directory | Example domain |
| --- | --- | --- |
| Presentation library | `.` | `talks.example.com` |
| Flutter monetization | `presentations/make-money-flutter-flutter-friends` | `flutter-monetization.talks.example.com` |
| Android monetization | `presentations/monetize-android-droidcon-usa-2026` | `android-monetization.talks.example.com` |
| How not to ship slop | `presentations/how-not-to-ship-slop` | `ship-slop.talks.example.com` |
| React Native monetization | `presentations/why-react-native-apps-monetize-better` | `react-native-monetization.talks.example.com` |

For each project:

1. Import this repository in Vercel.
2. Set **Root Directory** to the directory in the table.
3. Select **Other** as the Framework Preset and leave Build Command empty.
4. Deploy, then add the desired subdomain under **Settings → Domains**.
5. Enable **Skip deployment** for unaffected projects under the Root Directory
   settings if you do not want every repository push to redeploy every talk.

The `vercel.json` in each deployable directory enables clean URLs and always
redirects directory URLs to a trailing slash. The slash matters because each
deck deliberately uses relative paths for its images, fonts, and videos.

Use a specific CNAME-backed subdomain for each project. A Vercel wildcard
domain is only necessary if you later switch to a single dynamic project that
routes arbitrary hostnames; Vercel requires its nameservers for wildcard SSL.

### Adding another presentation

1. Create `presentations/<talk-slug>/` with a self-contained `index.html` and
   its assets.
2. Copy `vercel.json` and `.vercelignore` from an existing presentation and
   adjust the ignored source files if necessary.
3. Add the talk to the library in the root `index.html`.
4. Import the repository as another Vercel project, select the new directory as
   its Root Directory, and attach its subdomain.

## Presenting

- Left / Right, Page Up / Page Down, or Space: navigate
- Home / End: first or last slide
- `F`: fullscreen
- `N`: speaker notes
- `Q`: show or hide the audience QR code

For the most reliable local setup, run a static server from the repository root:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Talks

- [Why React Native apps monetize better — next.app devCon 2026](./presentations/why-react-native-apps-monetize-better/)
- [Make money with your Flutter app — Flutter & Friends](./presentations/make-money-flutter-flutter-friends/)
- [Monetize your Android app the right way — Droidcon USA 2026](./presentations/monetize-android-droidcon-usa-2026/)
- [AI doesn't ship slop. You do.](./presentations/how-not-to-ship-slop/)
