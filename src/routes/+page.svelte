<script>
  import EditorWindow from '$lib/EditorWindow.svelte';
</script>

<EditorWindow path="~/uchechi/home.svelte">
  <p class="font-mono text-sage text-sm mb-4">const developer =</p>
  <h1 class="font-mono text-4xl md:text-5xl font-bold leading-tight mb-4">
    Uchechi Cassandra<span class="cursor-blink text-amber">_</span>
  </h1>
  <p class="text-slate text-lg max-w-xl">
    Computer science student building toward full stack development. 90 days in, learning in public.
  </p>
  <div class="mt-8 flex gap-3 font-mono text-sm">
    <a href="/projects" class="px-4 py-2 rounded-lg bg-amber text-ink font-medium hover:opacity-90 transition">view projects</a>
    <a href="/about" class="px-4 py-2 rounded-lg border border-white/15 text-cream hover:border-amber/60 transition">about me</a>
  </div>
</EditorWindow>
