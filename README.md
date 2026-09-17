# midwestmusicICT

Website for **midwestmusicICT**, Kim Trujillo's live music booking business based in the Wichita, KS area.
Built with [Astro](https://astro.build) as a static site.

## Local development

```sh
npm install
npm run dev
```

Site runs at `http://localhost:4321`.

## Build

```sh
npm run build
```

Outputs static files to `dist/`.

## Deploying to Cloudflare Pages

The domain `midwestmusicict.com` is registered with Cloudflare. To deploy:

1. In the Cloudflare dashboard, go to **Workers & Pages → Create → Pages → Connect to Git**.
2. Select this repository and the `main` (or production) branch.
3. Build settings:
   - **Framework preset:** Astro
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
4. Deploy. Cloudflare Pages will build a preview URL for every pull request automatically, and deploy `main` to production.
5. Under the Pages project's **Custom domains**, add `midwestmusicict.com` (and `www.midwestmusicict.com`) — since the domain is already on Cloudflare, DNS records are added automatically.

## Content status

Real business content (bio copy, service packages, video/audio links, contact info) is still pending —
Kim is drafting a detailed content brief with another agent. See `CONTENT_TODO.md` for the current list of
placeholders to replace once that's ready.
