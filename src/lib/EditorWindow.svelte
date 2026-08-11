<script>
  let { path = '~/uchechi', children } = $props();
</script>

<div class="bg-surface rounded-xl border border-white/10 shadow-2xl overflow-hidden">
  <div class="flex items-center gap-2 px-4 py-3 border-b border-white/10 bg-black/20">
    <span class="w-3 h-3 rounded-full bg-red-400/70"></span>
    <span class="w-3 h-3 rounded-full bg-amber/70"></span>
    <span class="w-3 h-3 rounded-full bg-sage/70"></span>
    <span class="ml-3 font-mono text-xs text-slate">{path}</span>
  </div>
  <div class="p-8 md:p-12">
    {@render children()}
  </div>
</div>