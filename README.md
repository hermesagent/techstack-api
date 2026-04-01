# Tech Stack Detector API

Free API to detect technologies, frameworks, and tools used by any website. Identifies **219 technologies** across 19 categories including frameworks, CMS, analytics, CDN, security, and more.

**Version**: 1.3.0 | **Live API**: [hermesforge.dev/tools/techstack](https://hermesforge.dev/tools/techstack)

## Quick Start

```bash
# Detect technologies on a website
curl "https://hermesforge.dev/api/techstack?url=https://github.com"

# With API key for higher limits
curl -H "X-API-Key: YOUR_KEY" \
  "https://hermesforge.dev/api/techstack?url=https://shopify.com"
```

## Example Response

```json
{
  "url": "https://github.com",
  "technologies": [
    {
      "name": "Ruby on Rails",
      "category": "framework",
      "confidence": "medium"
    },
    {
      "name": "Turbo",
      "category": "js_library",
      "confidence": "medium"
    },
    {
      "name": "HSTS",
      "category": "security",
      "confidence": "high"
    }
  ],
  "_signatures": 219,
  "_version": "1.3.0"
}
```

## Technology Categories (19)

| Category | Count | Examples |
|----------|-------|---------|
| CMS | 31 | WordPress, Shopify, Docusaurus, GitBook, Notion |
| Widgets | 22 | Intercom, Algolia, Google Maps, Leaflet, Zendesk |
| JS Libraries | 21 | Redux, D3.js, GSAP, Socket.io, Moment.js |
| Platforms | 15 | Vercel, Firebase, Supabase, Deno Deploy |
| JS Frameworks | 19 | React, Vue, Angular, Svelte, Solid.js, Qwik |
| Servers | 12 | Nginx, Apache, LiteSpeed, Caddy, Envoy |
| Frameworks | 12 | Next.js, Django, Rails, Laravel, Astro |
| Analytics | 12 | GA4, Plausible, Amplitude, PostHog, Clarity |
| Marketing | 14 | Mailchimp, Facebook Pixel, ConvertKit, Klaviyo |
| CDN | 10 | Cloudflare, Fastly, CloudFront, jsDelivr |
| CSS Frameworks | 7 | Tailwind, Bootstrap, Bulma, Chakra UI |
| Monitoring | 7 | Sentry, Datadog, New Relic, Bugsnag |
| Build Tools | 6 | Webpack, Vite, Parcel, esbuild, Turbopack |
| Payment | 5 | Stripe, PayPal, Paddle, Gumroad, Braintree |
| Security | 4 | HSTS, CSP, X-Frame-Options |
| E-commerce | 4 | WooCommerce, Magento, BigCommerce |
| Auth | 4 | Auth0, Firebase Auth, Clerk, Supabase Auth |
| Optimization | 4 | Cloudinary, Imgix, Lazy Load |
| Hosting | 3 | GitHub Pages, Netlify, Cloudflare Pages |

## Rate Limits

| Tier | Rate | Daily | Monthly | Price |
|------|------|-------|---------|-------|
| No API key | 1/2 min | 10 | — | Free |
| Anonymous key (no email) | 1/2 min | 20 | — | Free |
| Free key (email verified) | 5/min | 50 | 500 | Free |
| Starter | 10/min | 200 | 2,000 | $4/30 days |
| Pro | 30/min | 1,000 | 10,000 | $9/30 days |
| Business | 60/min | 5,000 | 50,000 | $29/30 days |

Get an API key at [hermesforge.dev/api/keys](https://hermesforge.dev/api/keys) — no credit card required for free tiers.

## Use Cases

- **Competitive analysis** — See what tech your competitors use
- **Lead generation** — Find companies using specific technologies
- **Market research** — Understand technology adoption trends
- **Security auditing** — Identify outdated or vulnerable tech stacks
- **Sales intelligence** — Target prospects based on their tech stack
- **AI agent pipelines** — Enrich web research with technology context

## Other APIs by Hermes

| API | Description |
|-----|-------------|
| [Dead Link Checker](https://github.com/hermesagent/dead-link-checker) | Find broken links on any website |
| [Screenshot API](https://github.com/hermesagent/screenshot-api) | Capture full-page website screenshots |
| [Chart Rendering API](https://github.com/hermesagent/chart-rendering-api-visual-reporting-os) | Render Chart.js charts to PNG/JPEG |

## OpenAPI Spec

Available at: [hermesforge.dev/openapi/techstack](https://hermesforge.dev/openapi/techstack)

## License

MIT
