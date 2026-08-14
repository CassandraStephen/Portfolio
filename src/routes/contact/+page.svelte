<script>
  import EditorWindow from '$lib/EditorWindow.svelte';
</script>

<EditorWindow path="~/uchechi/contact.svelte">
  <p class="font-mono text-sage text-sm mb-4">// contact</p>
  <h1 class="font-mono text-3xl font-bold mb-6">Get In Touch</h1>
  <p class="text-slate mb-8 max-w-xl">Have a question or project idea? Send a message below.</p>

  <form action="https://formspree.io/f/mvkpqkjk" method="POST" class="max-w-xl space-y-4">
    <div>
      <label for="name" class="block font-mono text-xs text-slate mb-1">Name</label>
      <input type="text" id="name" name="name" required
        class="w-full bg-black/30 border border-white/10 rounded-md px-3 py-2 text-cream focus:outline-none focus:border-amber/60 transition" />
    </div>
    <div>
      <label for="email" class="block font-mono text-xs text-slate mb-1">Email</label>
      <input type="email" id="email" name="email" required
        class="w-full bg-black/30 border border-white/10 rounded-md px-3 py-2 text-cream focus:outline-none focus:border-amber/60 transition" />
    </div>
    <div>
      <label for="message" class="block font-mono text-xs text-slate mb-1">Message</label>
      <textarea id="message" name="message" rows="5" required
        class="w-full bg-black/30 border border-white/10 rounded-md px-3 py-2 text-cream focus:outline-none focus:border-amber/60 transition"></textarea>
    </div>
    <button type="submit" class="px-5 py-2 rounded-lg bg-amber text-ink font-mono text-sm font-medium hover:opacity-90 transition">
      Let's Connect
    </button>
  </form>
</EditorWindow>