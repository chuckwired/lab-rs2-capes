# lab-rs2-capes

Interactive showcase of RuneScape skill capes. They float in a dark void; click one to bring it forward and tilt it in 3D with the mouse (or drag on touch). Esc or a click elsewhere puts it back.

Static site: one `index.html`, no build step, no dependencies. The capes are drawn as layered SVG in the script, so there are no image assets.

## Run

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

## Configure

Everything tunable is in the `CONFIG` object at the top of the script:

- `defaultShown`: which capes show on first visit (the picker, top right, remembers the choice)
- `capeStyle`: art style per cape; herblore has `rs3` and `osrs`
- drift, tilt limits, glow, blur, spring and shooting-star timings

## Hosting

Any static host works (GitHub Pages, Cloudflare Pages, Netlify, nginx). The only external request is Google Fonts (Instrument Serif, JetBrains Mono, Jersey 10); self-host them if you want zero third-party calls.

## Credits

Fan project, non-commercial. RuneScape is a trademark of Jagex Ltd; the cape designs are redrawn from reference and are not Jagex assets.
