<script>
	import Table from "$lib/Table.svelte";


</script>


<div class="relative pt-16 pb-20 px-4 sm:px-6 lg:pt-24 lg:pb-28 lg:px-8 font-proxima">
    <div class="absolute inset-0">
        <div class="bg-white h-1/3 sm:h-2/3"></div>
    </div>
    <div class="relative max-w-7xl mx-auto">
        <Table 
            title="All Categories"
            description="Check out our complete list of Categories."
            name="Category Name"
            link="/categories"
        />
    </div>
</div>