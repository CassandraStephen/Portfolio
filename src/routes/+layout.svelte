<script>
  import '../app.css';
  import { page } from '$app/stores';
  let {children} = $props();
  const tabs = [
    { href: '/', label: 'home.svelte' },
    { href: '/about', label: 'about.svelte' },
    { href: '/projects', label: 'projects.svelte' }
  ];
</script>

<div class="min-h-screen bg-ink text-cream font-sans selection:bg-amber selection:text-ink">
  <header class="border-b border-white/10 bg-surface/60 backdrop-blur">
    <nav class="max-w-4xl mx-auto flex px-4">
      {#each tabs as tab}
        <a
          href={tab.href}
          class="font-mono text-sm px-4 py-3 border-b-2 transition-colors
            {$page.url.pathname === tab.href ? 'border-amber text-amber' : 'border-transparent text-slate hover:text-cream'}"
        >
          {tab.label}
        </a>
      {/each}
    </nav>
  </header>
  <main class="max-w-4xl mx-auto px-4 py-12">
    {@render children()}
  </main>
</div>