<script>
	import Button from "./Ui/Button.svelte";
</script>

<div class="px-4 sm:px-10 lg:px-12 text-center lg:max-w-5xl mx-auto mb-8 pb-20 lg:pb-24">
    <h1 class="font-bebas text-3xl uppercase tracking-widest text-blue-900 mb-8 lg:mb-18">About American Made Products</h1>
    <p class="font-proxima text-lg tracking-wide text-gray-700 leading-8 pb-8">
        We believe that if enough of us buy American we can boost the US economy, increase American jobs, create better working conditions, and help the environment. Our goal is to provide you with many options for products made in the USA and keep the list as accurate as possible.
    </p>
    <div class="mt-12 lg:mt-18">
        <Button
            href="/search"
            text="Search American Products"
        />
    </div>
</div>