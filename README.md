# Memory Keep

Website for **Memory Keep**, a small film-slide digitization business in Gilbert, Arizona. Instead of scanning, each slide is rephotographed with a professional camera, macro lens, and precision lighting.

Live site: [memorykeep.us](https://memorykeep.us)

## Tech

Plain HTML and CSS, no build step and no dependencies. Hosted on GitHub Pages.

| Page | File |
| --- | --- |
| Home | `index.html` |
| Services | `services.html` |
| Steps | `steps.html` |
| Testimonial | `testimonial.html` |
| Gallery | `gallery.html` |
| Contact | `contact.html` (form via [Formspree](https://formspree.io)) |

Shared styles live in `style.css`. The layout is responsive, with a hamburger menu on small screens.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**, set **Source** to "Deploy from a branch", choose `main` and `/ (root)`.
3. The `CNAME` file points the site at `memorykeep.us`. At your domain registrar, add the DNS records GitHub lists for custom domains, then turn on **Enforce HTTPS**.

`.nojekyll` tells Pages to serve the files as-is.

## Adding gallery photos

1. Resize the photo to about 2000 px wide and save it in `gallery/` as the next number (for example `66.jpg`).
2. In `gallery.html`, copy the last `<a href="gallery/65.jpg">…</a>` entry and change the number.
3. Commit and push. The site updates in about a minute.

## Still to do

- Orders come in through the contact form (service + number of sets). Payment is arranged by reply; there is no online checkout.

## License

© 2026 Memory Keep. All rights reserved. Photos and copy may not be reused without permission.
