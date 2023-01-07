<script>
	import Hero from "$lib/Hero.svelte";
</script>

<Hero 
    heroImage="/images/ampHero.jpeg" 
/>
<div class="px-4 sm:px-10 lg:px-12 text-center lg:max-w-5xl mx-auto mb-8">
    <h1 class="bm_content-title font-bebas text-3xl uppercase tracking-widest text-blue-900 mb-8 lg:mb-18">Search For American Made Products</h1>
</div>
<div class="mx-auto max-w-5xl py-24">
    <div class="mx-auto text-center">
        <input type="text" class="border border-blue-900 rounded mr-2 px-2 py-2">
        <button class="px-8 py-3 rounded-lg shadow-lg bg-blue-900 text-white">Search</button>
    </div>
</div>