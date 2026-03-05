# Tech Stack Detector API

Free API to detect technologies, frameworks, and tools used by any website. Identifies 155+ technologies across categories like frameworks, CMS, analytics, CDN, and more.

**Live API**: [51-68-119-197.sslip.io/tools/techstack](https://51-68-119-197.sslip.io/tools/techstack)

## Quick Start

```bash
# Detect technologies on a website
curl "https://51-68-119-197.sslip.io/api/techstack?url=https://github.com"

# With API key for higher limits
curl -H "X-API-Key: YOUR_KEY" \
  "https://51-68-119-197.sslip.io/api/techstack?url=https://shopify.com"
```

## Example Response

```json
{
  "url": "https://github.com",
  "technologies": [
    {
      "name": "React",
      "category": "js_framework",
      "confidence": 0.9
    },
    {
      "name": "Node.js",
      "category": "backend",
      "confidence": 0.8
    },
    {
      "name": "Webpack",
      "category": "build_tool",
      "confidence": 0.85
    }
  ],
  "meta": {
    "title": "GitHub",
    "generator": null,
    "server": "GitHub.com"
  }
}
```

## Technology Categories

| Category | Examples |
|----------|----------|
| `framework` | React, Vue.js, Angular, Next.js, Nuxt.js |
| `cms` | WordPress, Drupal, Joomla, Ghost |
| `analytics` | Google Analytics, Plausible, Matomo |
| `cdn` | Cloudflare, Fastly, AWS CloudFront |
| `hosting` | Vercel, Netlify, GitHub Pages |
| `ecommerce` | Shopify, WooCommerce, Magento |
| `css_framework` | Tailwind CSS, Bootstrap, Bulma |
| `build_tool` | Webpack, Vite, Parcel |
| `backend` | Node.js, PHP, Django, Rails |
| `server` | Nginx, Apache, LiteSpeed |

## Rate Limits

| Tier | Limit |
|------|-------|
| No API key | 2 requests/minute |
| Free API key | 5 requests/minute, 50/day |

Get a free API key at [51-68-119-197.sslip.io/tools/techstack](https://51-68-119-197.sslip.io/tools/techstack).

## Use Cases

- **Competitive analysis** - See what tech your competitors use
- **Lead generation** - Find companies using specific technologies
- **Market research** - Understand technology adoption trends
- **Security auditing** - Identify outdated or vulnerable tech stacks
- **Sales intelligence** - Target prospects based on their tech stack

## Other APIs by Hermes

| API | Description |
|-----|-------------|
| [Dead Link Checker](https://github.com/hermesagent/dead-link-checker) | Find broken links on any website |
| [Screenshot API](https://github.com/hermesagent/screenshot-api) | Capture full-page website screenshots |
| [SSL Certificate Checker](https://51-68-119-197.sslip.io/tools/ssl) | Validate SSL certificates |
| [SEO Analyzer](https://51-68-119-197.sslip.io/tools/seo) | Analyze on-page SEO factors |
| [Performance Audit](https://51-68-119-197.sslip.io/tools/performance) | Page load speed analysis |

## OpenAPI Spec

Available at: [/openapi/techstack](https://51-68-119-197.sslip.io/openapi/techstack)

## License

MIT
