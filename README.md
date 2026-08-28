# The Grinch Towing — homepage rebuild (demo)

Static, dependency-free rebuild of the Wix homepage for
**The Grinch Towing**, Indian Trail NC — specialty flatbed transport
for low-clearance and exotic vehicles.

## Why it is fast

| | |
|---|---|
| Total page weight | ~308 KB (mobile ~213 KB) |
| HTTP requests | 10 |
| JavaScript | 12 lines, inline (mobile menu only) |
| CSS | inline in `<head>`, zero render-blocking requests |
| Fonts | Wix Madefor, self-hosted WOFF2, preloaded |
| Images | WebP, explicit width/height, lazy below the fold |

Measured in headless Chromium, mobile profile (4x CPU throttle, Slow 4G):

```
DESKTOP  FCP   64ms   LCP   64ms   CLS 0
MOBILE   FCP  448ms   LCP 1124ms   CLS 0.0114
```

## Note on the images

Every image here was recovered from screenshots of the live Wix site, then
cleaned up (the baked-in headline and buttons were painted out so the real
HTML text could sit on top). They are placeholders at screenshot resolution.
Swapping in the originals from the Wix media manager is a drop-in replacement
and will sharpen the page considerably.

The "How It Works" panel is a poster frame — the original is a 22-second
video and will be restored as a self-hosted, lazy-loaded `<video>`.
