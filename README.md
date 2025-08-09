# Muscarelli Auction Company — Single-Page Website

A modern, SEO-friendly single page for Muscarelli Auction Company (Hickory, NC).  
Built with plain HTML, and vanilla JS. Deployed automatically to Netlify on every push to `main`.

![Repository Preview](images/footer-logo.jpg)

## Features

- Single `index.html` file
- SEO-ready meta tags
- Open Graph + Twitter Card
- Local business + FAQ JSON-LD
- Responsive design with Tailwind
- Netlify Forms with honeypot + reCAPTCHA
- Smooth scrolling and mobile navigation
- Editable featured auctions and videos

## Deployment

This repo deploys automatically to **Netlify** on push to `main`.

**Netlify settings:**

- **Build command:** none
- **Publish directory:** `/`
- **Forms:** auto-detected

## Local Development

No build step required—just open `index.html`.  
For a local server:

```bash
# Python
python3 -m http.server 8080

# Node
npx serve -p 8080
```

Visit: http://localhost:8080

index.html file can also be opened in the browser in case you aren't using a server.

## Project Structure

```
.
├─ index.html
└─ images/
   └─ footer-logo.jpg
```

## Editing Content

- **Auctions:** update `auctions` array in `loadAuctions()`
- **Videos:** update `videos` array in `loadVideos()`
- **Contact info:** update visible text + JSON-LD block
- **Social images:** update `og:image` and `twitter:image`

## Forms

The contact form uses Netlify:

```html
<form
  name="muscarelli-contact"
  method="POST"
  data-netlify="true"
  netlify-honeypot="bot-field"
  data-netlify-recaptcha="true"
></form>
```

Submissions appear in Netlify → Forms.

## Contributing

1. Create a branch
2. Edit `index.html`
3. Open a PR — merging to `main` triggers deployment

## License

MIT © Muscarelli Auction Company
