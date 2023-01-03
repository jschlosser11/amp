<script>
	import AboutAmp from "$lib/AboutAmp.svelte";
	import FeatureBlog from "$lib/FeatureBlog.svelte";
	import Hero from "$lib/Hero.svelte";
	import Share from "$lib/Share.svelte";
	import WhyAmp from "$lib/WhyAmp.svelte";
</script>

<div>
	<div>
		<Hero heroImage="/images/ampHero.jpeg" />
	</div>
	<div>
		<AboutAmp />
	</div>
	<div>
		<WhyAmp />
	</div>
	<div>
		<Share />
	</div>
	<div>
		<FeatureBlog />
	</div>
</div>
