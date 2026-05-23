# Code Keylight

A fake, animated **"AI is coding"** screen you can use as a **key light** for video.

Throw it fullscreen on a monitor or tablet next to your camera: the bright screen
lights up your face, and the reflection — especially in glasses — reads as live
code being written. You look like you're deep in the matrix; it's really just a
lamp that happens to look like an IDE. 😎

> **Live demo:** _drop your hosted link here_

## Use it

1. Open `index.html` in any browser. No build step, no dependencies, works offline.
2. Press **F** for fullscreen.
3. Press **R** for **reflection mode** — big, bold, high-contrast code that stays
   legible when it's shrunk down in a glasses reflection.
4. Tune it to your setup with the keys below.

### Keyboard controls

| Key        | Action                                            |
| ---------- | ------------------------------------------------- |
| `F`        | Fullscreen                                        |
| `R`        | Reflection mode (big, bold, high-contrast)        |
| `[` / `]`  | Shrink / grow font size (also `↑` / `↓`)          |
| `D`        | Toggle light / dark theme                         |
| `B`        | Brightness boost (cycles a white glow overlay)    |
| `+` / `-`  | Typing speed                                      |
| `?`        | Show / hide the controls (hidden by default while recording) |

**Tip:** the light theme throws the most light on your face; the dark theme reads
as "code" most clearly in a reflection but lights you less. Try both and see what
your camera prefers, and crank your display brightness all the way up.

## Make it yours

Open `index.html` and edit the `BRAND` block near the top of the `<script>`:

```js
const BRAND = {
  name: "Code Keylight",
  tagline: "A fake AI coding screen, bright enough to light you up on camera.",
  credit: "Built by Biz Cannon",   // shows small on the intro splash — set "" to hide
  showSplash: true                // brief intro that fades out before you record
};
```

Swap `logo.png` for your own to rebrand the splash and favicon. Want different code
scrolling on screen? Edit the `files` array right below the config — each entry is
just a filename and a string of code.

## Host it

It's plain static files (`index.html` + `logo.png`), so it'll run anywhere — just
keep them in the same folder:

- **GitHub Pages** — push this repo, turn on Pages, done.
- **Netlify / Vercel / Cloudflare Pages** — drag the folder into the dashboard.
- **Locally** — just double-click `index.html`.

## Privacy

No analytics, no network requests, no cookies — nothing phones home. Everything
runs in your browser, and the page works fully offline.

## License

[MIT](LICENSE). Free to use, fork, and modify.

---

Built by **Biz Cannon**.
