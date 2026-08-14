<script>
  import EditorWindow from '$lib/EditorWindow.svelte';
  const skills = ['SvelteKit', 'Tailwind CSS', 'Auth', 'PostgreSQL', 'TypeScript/JavaScript', 'React'];
</script>

<EditorWindow path="~/uchechi/about.svelte">
  <p class="font-mono text-sage text-sm mb-4">// about</p>
  <h1 class="font-mono text-3xl font-bold mb-6">About Me</h1>
  <p class="text-slate text-lg leading-relaxed mb-10 max-w-xl">
    I'm Uchechi Cassandra, a computer science student with a passion for science and technology.
    I'm on a 90-day journey to becoming a full stack web developer, building real projects along the way.<br>
  
  <h2 class="font-mono text 2xl font-bold mb-6"> Background Story</h2>
    <p>I remember starting this journey with much anxiety, but was expectant and curious anyway, never knew i could have a deployable site to 
    my name. This is the stepping stone for a better skillset and finally jumping off the cliff of uncertainty into the river of self-trust and gaining client trust 
    through real projects and intense learning. </p><br>
    <p> A big shout out to the Zero to Hired Platform and Our amiable guide Wilson Wilson, who has selflessly gone out of his way to help us improve in our skills.


  </p><br>


  <p class="font-mono text-sage text-sm mb-3"> //my expertise</p>
  <ul class="flex flex-wrap gap-2">
    {#each skills as skill}
      <li class="font-mono text-sm px-3 py-1.5 rounded-md bg-black/30 border border-white/10 text-cream">{skill}</li>
    {/each}
  </ul>

  <p class="font-mono text-sage text-sm mb-3 mt-10">// poetry</p>
  <div class="space-y-5">
    <a href="https://substack.com/profile/537276313-uchechi-cassandra/note/c-314362403?r=8vvp21" class="block border-l-2 border-sage/40 hover:border-amber pl-4 py-1 transition group">
      <p class="text-cream italic leading-relaxed mb-1">"Silver screens unfurl like tapestries of dreams...."</p>
      <p class="font-mono text-xs text-slate group-hover:text-amber transition">Reel Romance →</p>
    </a>

     <a href="https://substack.com/profile/537276313-uchechi-cassandra/note/c-314362160?r=8vvp21" class="block border-l-2 border-sage/40 hover:border-amber pl-4 py-1 transition group">
      <p class="text-cream italic leading-relaxed mb-1">"I was caught in a free web, my heart dicky with anxiety...."</p>
      <p class="font-mono text-xs text-slate group-hover:text-amber transition">Big little things →</p>
    </a>

    <a href="https://substack.com/profile/537276313-uchechi-cassandra/note/c-314368328?r=8vvp21" class="block border-l-2 border-sage/40 hover:border-amber pl-4 py-1 transition group">
      <p class="text-cream italic leading-relaxed mb-1">"I prefer you to a bowel of gizzard...."</p>
      <p class="font-mono text-xs text-slate group-hover:text-amber transition">A message to music →</p>
    </a>

    <a href="https://substack.com/profile/537276313-uchechi-cassandra/note/c-314368527?r=8vvp21" class="block border-l-2 border-sage/40 hover:border-amber pl-4 py-1 transition group">
      <p class="text-cream italic leading-relaxed mb-1">"Do not be anxious about the next day, my bible would always say.."</p>
      <p class="font-mono text-xs text-slate group-hover:text-amber transition">Survival Stings →</p>
    </a> 
    <br>
    <p><em> ...and lots more if <a href="https://uchechicassandra.substack.com"> you visit here!</a></em></p>
  </div>
</EditorWindow>