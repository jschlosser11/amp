<script>
	import Table from "$lib/Table.svelte";
    export let data;
</script>
<div class="relative pt-16 pb-20 px-4 sm:px-6 lg:pt-24 lg:pb-28 lg:px-8 font-proxima">
    <div class="absolute inset-0">
        <div class="bg-white h-1/3 sm:h-2/3"></div>
    </div>
    <div class="relative max-w-7xl mx-auto">
        <Table 
            title="American Made Brands"
            description="Check out a full list of brands that manufacture their products right here in the USA."
            name="Brand Name"
            link="/brands"
        />
    </div>
</div>  