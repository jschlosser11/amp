<script>
    let useful = [
                {
                    name: 'Home',
                    link: '/'
                },
                {
                    name: 'Brands',
                    link: '/brands'
                },
                {
                    name: 'Categories',
                    link: '/categories'
                },
                {
                    name: 'Blog',
                    link: 'blog'
                }
    ]
    let popular = [
                {
                    name: 'Channel Lock',
                    link: '#'
                },
                {
                    name: 'Armour All',
                    link: '#'
                },
                {
                    name: 'Bison Coolers',
                    link: '#'
                },
                {
                    name: "Charlie's Soap",
                    link: '#'
                },
                {
                    name: "Zippo",
                    link: '#'
                }
    ]
</script>

<footer class="bg-gray-100">
    <h2 class="sr-only">Footer</h2>
    <div class="max-w-7xl mx-auto pt-12 px-4 sm:px-6 lg:pt-16 lg:px-8">
        <div class="xl:grid xl:grid-cols-3 xl:gap-8">
            <div class="space-y-4 xl:col-span-1">
                <img src="/images/ampLogo.png" alt="amp-logo" class="h-20">
                <span class="block text-blue-900 text-sm font-semibold">Amazon Affiliate</span>
                <p class="text-gray-500 text-sm">American-Made-Products.info is a participant in the Amazon Associates Program, an affiliate advertising program designed to provide a means for sites to earn advertising fees by advertising and linking to Amazon.com. We use these fees to help pay for hosting, maintenance, and keeping the content of the site as up to date as possible.</p>
                <div class="flex space-x-6">
                    <a href="https://www.facebook.com/americanmadeproducts1/" class="text-gray-400 hover:text-gray-500">
                        <span class="sr-only">Facebook</span>
                        <svg class="h-6 w-6 text-blue-900 hover:text-blue-600" fill="currentcolor" viewBox="0 0 24 24" aria-hidden="true">
                            <path fill-rule="evenodd" d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094.0 2.238.195 2.238.195v2.46h-1.26c-1.243.0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z" clip-rule="evenodd"></path>
                        </svg>
                    </a>
                </div>
            </div>
            <div class="mt-12 grid grid-cols-2 gap-8 xl:mt-0 xl:col-span-2 xl:pl-24">
                    <div>
                        <div class="mt-12 md:mt-0">
                            <h3 class="text-sm font-semibold text-blue-900 tracking-wider uppercase">Useful Links</h3>
                            {#each useful as data}
                                <ul class="mt-4 space-y-4">
                                    <li>
                                        <a href={data.link} class="text-base text-gray-500 hover:text-gray-900">{data.name}</a>
                                    </li>
                                </ul>
                            {/each}
                        </div>
                    </div>
                     <div>
                        <div class="mt-12 md:mt-0">
                            <h3 class="text-sm font-semibold text-blue-900 tracking-wider uppercase">Popular</h3>
                            {#each popular as data}
                                <ul class="mt-4 space-y-4">
                                    <li>
                                        <a href={data.link} class="text-base text-gray-500 hover:text-gray-900">{data.name}</a>
                                    </li>
                                </ul>
                            {/each}
                        </div>
                    </div>
               
            </div>
        </div>
    </div>
    <div class="mt-12 border-t border-gray-200 py-8 text-center bg-blue-900">
        <p class="text-base text-white xl:text-center">Made Proudly in America by ?? 2021 American-Made-Products.info</p>
    </div>

</footer>