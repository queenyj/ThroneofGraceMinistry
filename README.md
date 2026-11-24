# Throne of Grace Ministry

Run these commands from the project folder with Node.js 22.12 or later and npm installed.

```sh
npm install
npm run dev
```

Open [the development server](http://localhost:4321) for live updates. Use the URL Astro prints if the port is already in use.

To preview the production build locally, stop the development server with Ctrl+C and run:

```sh
npm run build
npm run preview
```

The static build goes to `dist/`. Cloudflare Workers reads [wrangler.jsonc](wrangler.jsonc) to serve that directory through Static Assets. If you connect the repository to Workers Builds, set the build command to `npm run build`.

To enable the Contact page’s email link, set `MINISTRY_CONTACT_EMAIL` to the ministry’s public email address in a local `.env` file or in the deployment build environment. Astro embeds the address in the page at build time.
