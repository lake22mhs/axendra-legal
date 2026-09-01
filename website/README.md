# Axendra website

This is a dependency-free static landing page for driving web visitors to the Axendra iPhone app.

## Local preview

From the repository root:

```sh
npx serve website
```

The App Store CTA currently points to an Axendra search URL because the final App Store product URL has not been confirmed. Replace that single link in `website/index.html` once the app listing is live.

The page intentionally has no analytics SDK or form backend yet. Add consent-gated, privacy-safe measurement only after the production website domain and analytics plan are approved.

## Google Search readiness

The page includes an index/follow robots directive, canonical URL, Open Graph and Twitter metadata, JSON-LD SoftwareApplication structured data, and a sitemap. `robots.txt` allows public crawling.

The production domain is `https://axendra.fyi/`. After deployment, verify the live URL in Google Search Console and submit `https://axendra.fyi/sitemap.xml`. Do not publish the local `file://` preview URL: Google can only crawl the publicly hosted HTTPS site.
