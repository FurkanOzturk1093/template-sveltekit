# DeployWise — SvelteKit Template

A production-ready SvelteKit starter, pre-configured for one-click deployment to your VPS with [DeployWise](https://deploywise.dev).

## What's Included

- SvelteKit with TypeScript
- Vite-powered dev server
- adapter-node ready for PM2 deployment

## Quick Start

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173).

## Deploy with DeployWise

1. Push this repo to GitHub
2. Open [deploywise.dev/dashboard](https://deploywise.dev/dashboard)
3. Add your VPS → Create a project → Select this repo
4. Click **Deploy**

DeployWise automatically runs `vite build`, starts with PM2 (via adapter-node), configures Nginx, and issues a free SSL certificate.

## Project Structure

```
├── src/
│   ├── routes/
│   │   └── +page.svelte  # Home page
│   └── app.html           # HTML template
├── svelte.config.js       # SvelteKit config
├── vite.config.ts         # Vite config
└── package.json
```

## Learn More

- [Deploy SvelteKit to VPS Guide](https://deploywise.dev/guides/deploy-sveltekit-to-vps)
- [DeployWise Docs](https://deploywise.dev/docs)
- [SvelteKit Documentation](https://svelte.dev/docs/kit)

---

Deployed with [DeployWise](https://deploywise.dev) — free, open source.
