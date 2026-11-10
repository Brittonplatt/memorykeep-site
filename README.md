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

## Still to do

- Replace `YOUR_FORM_ID` in `contact.html` with your Formspree form ID.
- Set up a way to take orders and payment. The "Order Now" buttons currently go to the contact page (the old Pixieset store goes away with Pixieset).

## License

© 2026 Memory Keep. All rights reserved. Photos and copy may not be reused without permission.
