<script>
  import EditorWindow from '$lib/EditorWindow.svelte';
</script>

<EditorWindow path="~/uchechi/projects.svelte">
  <p class="font-mono text-sage text-sm mb-6">// projects</p>
  <div class="border border-white/10 rounded-lg p-6 mb-4 hover:border-amber/40 transition">
    <h2 class="font-mono text-xl font-semibold mb-2">Personal Portfolio Website</h2>
    <p class="text-slate mb-3">This very site — built from scratch to showcase my journey into full stack development.</p>
    <p class="font-mono text-xs text-sage">SvelteKit · Tailwind CSS</p>
  </div>
  <div class="border border-white/5 rounded-lg p-6 mb-4 opacity-40">
    <h2 class="font-mono text-xl font-semibold mb-2">Coming Soon</h2>
    <p class="text-slate">More projects on the way as I keep building.</p>
  </div>
  <div class="border border-white/5 rounded-lg p-6 opacity-40">
    <h2 class="font-mono text-xl font-semibold mb-2">Coming Soon</h2>
    <p class="text-slate">More projects on the way as I keep building.</p>
  </div>
</EditorWindow>