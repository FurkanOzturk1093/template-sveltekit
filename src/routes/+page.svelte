<svelte:head>
  <title>SvelteKit App — Deployed with DeployWise</title>
  <meta name="description" content="A SvelteKit starter template deployed on your own VPS with DeployWise." />
</svelte:head>

<main class="page">
  <!-- Glow -->
  <div class="glow"></div>

  <!-- Live badge -->
  <div class="live-badge">
    <span class="pulse-dot"></span>
    Live on DeployWise
  </div>

  <!-- Framework badge -->
  <div class="framework-badge">SvelteKit · Svelte</div>

  <!-- Heading -->
  <h1 class="heading">Your app is live. 🚀</h1>

  <p class="description">
    This SvelteKit starter is deployed and running on your own VPS.
    Edit <code>src/routes/+page.svelte</code> to get started.
  </p>

  <!-- CTA -->
  <a href="https://deploywise.dev" target="_blank" rel="noopener noreferrer" class="cta">
    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
      <path d="M22 12h-4l-3 9L9 3l-3 9H2"/>
    </svg>
    Deployed with DeployWise
    <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
      <path d="M7 17L17 7M7 7h10v10"/>
    </svg>
  </a>
</main>

<style>
  @keyframes pulse {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.4; }
  }

  :global(*) { box-sizing: border-box; margin: 0; padding: 0; }
  :global(body) { background: #0a0a0a; }

  .page {
    min-height: 100vh;
    background: linear-gradient(135deg, #0a0a0a 0%, #111827 50%, #0a0a0a 100%);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    color: #fff;
    padding: 2rem;
    position: relative;
    overflow: hidden;
  }

  .glow {
    position: absolute;
    top: 20%;
    left: 50%;
    transform: translateX(-50%);
    width: 600px;
    height: 300px;
    background: radial-gradient(ellipse, rgba(255, 62, 0, 0.12) 0%, transparent 70%);
    pointer-events: none;
  }

  .live-badge {
    display: flex;
    align-items: center;
    gap: 8px;
    background: rgba(16, 185, 129, 0.1);
    border: 1px solid rgba(16, 185, 129, 0.3);
    border-radius: 999px;
    padding: 6px 16px;
    margin-bottom: 2.5rem;
    font-size: 13px;
    color: #10b981;
  }

  .pulse-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    background: #10b981;
    display: inline-block;
    box-shadow: 0 0 8px #10b981;
    animation: pulse 2s infinite;
  }

  .framework-badge {
    background: rgba(255, 255, 255, 0.06);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 12px;
    padding: 8px 20px;
    margin-bottom: 1.5rem;
    font-size: 13px;
    color: rgba(255, 255, 255, 0.5);
    letter-spacing: 0.08em;
    text-transform: uppercase;
    font-weight: 600;
  }

  .heading {
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    font-weight: 800;
    margin: 0 0 1rem;
    text-align: center;
    line-height: 1.1;
    background: linear-gradient(135deg, #fff 30%, rgba(255, 255, 255, 0.5));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .description {
    font-size: 1.125rem;
    color: rgba(255, 255, 255, 0.45);
    text-align: center;
    max-width: 480px;
    line-height: 1.7;
    margin: 0 0 3rem;
  }

  .description code {
    background: rgba(255, 255, 255, 0.08);
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 0.9em;
    color: rgba(255, 255, 255, 0.7);
  }

  .cta {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: rgba(255, 62, 0, 0.12);
    border: 1px solid rgba(255, 62, 0, 0.35);
    color: #fb923c;
    border-radius: 12px;
    padding: 14px 28px;
    text-decoration: none;
    font-size: 15px;
    font-weight: 600;
    transition: all 0.2s;
  }

  .cta:hover {
    background: rgba(255, 62, 0, 0.22);
    border-color: rgba(255, 62, 0, 0.6);
  }
</style>
