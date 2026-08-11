<script>
  import EditorWindow from '$lib/EditorWindow.svelte';
  const skills = ['SvelteKit', 'Tailwind CSS', 'Auth', 'PostgreSQL', 'TypeScript'];
</script>

<EditorWindow path="~/uchechi/about.svelte">
  <p class="font-mono text-sage text-sm mb-4">// about</p>
  <h1 class="font-mono text-3xl font-bold mb-6">About Me</h1>
  <p class="text-slate text-lg leading-relaxed mb-10 max-w-xl">
    I'm Uchechi Cassandra, a computer science student with a passion for science and technology.
    I'm on a 90-day journey to becoming a full stack web developer, building real projects along the way.
  </p>
  <p class="font-mono text-sage text-sm mb-3">// stack</p>
  <ul class="flex flex-wrap gap-2">
    {#each skills as skill}
      <li class="font-mono text-sm px-3 py-1.5 rounded-md bg-black/30 border border-white/10 text-cream">{skill}</li>
    {/each}
  </ul>
</EditorWindow>