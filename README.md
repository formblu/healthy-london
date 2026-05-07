# Healthy London

An interactive data visualization exploring **healthy life expectancy** across London's five NHS Integrated Care Boards (ICBs): North West, North Central, North East, South East, and South West London.

The headline question: people may be living longer, but how many of those years are spent in good health?

## What's here

- `index.html` — single-file static app (vanilla HTML / CSS / SVG / JavaScript, no frameworks, no build step)
- `slides/` — seven Insights infographic JPGs

## Pages

- **Map** — interactive choropleth showing HLE, LE, and the gap between them across the five ICBs. Filter by gender, age, and metric. Click any ICB for trend sparklines and key insights.
- **Insights** — seven infographic slides exploring the data narrative.
- **Methodology** — how the data was sourced and assembled, with caveats.
- **About** — project credit and contact.

## Data sources

All data comes from the **UK Office for National Statistics**, released under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/):

- Life expectancy for local areas of the UK (released Dec 2025)
- Healthy life expectancy, UK (released Feb 2026)
- Population estimates for 2024 ICBs

## Local development

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/ in your browser.

(Direct `file://` opening of `index.html` won't load images correctly because of browser security restrictions on local-file requests — always serve via a local HTTP server.)

## Deployment

Static site. Any modern static host works (Vercel, Netlify, Cloudflare Pages, GitHub Pages, S3, etc.). No build step required.

## Credits

Designed and built by [Nazia Parvez](https://www.linkedin.com/in/naziaparvez/).
