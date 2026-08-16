<script>
  import SocialLinks from '$lib/SocialLinks.svelte';
  import '../app.css';
  import { page } from '$app/stores';
  import Home from '@lucide/svelte/icons/home';
  import User from '@lucide/svelte/icons/user';
  import FolderGit2 from '@lucide/svelte/icons/folder-git-2';
  import Mail from '@lucide/svelte/icons/mail';
  let { children } = $props();
  const tabs = [
    { href: '/', label: 'home', icon: Home },
    { href: '/about', label: 'about', icon: User },
    { href: '/projects', label: 'projects', icon: FolderGit2 },
    { href: '/contact', label:'contact', icon: Mail},
  ];
</script>

<div class="min-h-screen bg-ink text-cream font-sans selection:bg-amber selection:text-ink">
  <header class="border-b border-white/10 bg-surface/60 backdrop-blur">
    <nav class="max-w-4xl mx-auto flex px-2 sm:px-4">
  {#each tabs as tab}
    <a
      href={tab.href}
      class="flex items-center justify-center sm:justify-start gap-1.5 sm:gap-2 font-mono text-xs sm:text-sm px-2.5 sm:px-4 py-3 border-b-2 flex-1 sm:flex-none transition-colors
        {$page.url.pathname === tab.href ? 'border-amber text-amber' : 'border-transparent text-slate hover:text-cream'}"
    >
      <tab.icon size={16} />
      <span class="hidden sm:inline">{tab.label}</span>
    </a>
  {/each}
</nav>
  </header>
  <main class="max-w-4xl mx-auto px-4 py-12">
    {@render children()}
  </main>

   <footer class="border-t border-white/10 mt-12 py-8 flex flex-col items-center gap-3">
    <SocialLinks size={16} />
    <p class="font-mono text-xs text-slate">© {new Date().getFullYear()} Uchechi Cassandra</p>
  </footer>
</div>