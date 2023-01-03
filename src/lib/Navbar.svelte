<script>
    let navLinks = [
        {
            name: 'Home',
            link: '/',
        },
        {
            name: 'All Brands',
            link: '/brands',
        },
        {
            name: 'Categories',
            link: '/categories',
        },
        {
            name: 'Search',
            link: '/search',
        },
        {
            name: 'Blog',
            link: '/blog',
        },
        {
            name: 'Contact',
            link: '/contact',
        },
    ]

    let open = false;

    const opened = () => {
        open = true;
    }
     const closed = () => {
        open = false;
    }
</script>
<div class="bg-white border-b-4 border-blue-900 sticky top-0 mx-auto w-full z-50">
    <div class="bg-white flex lg:max-w-screen-xl lg:mx-auto">
        <div class="py-4 px-4 pl-8">
            <a href="/">
                <img src="/images/ampLogo.png" class="h-32 w-auto" alt="amp-logo">
            </a>
        </div>
        <div class="px-4 sm:px-6 hidden md:block md:flex-grow">
            <nav class="sm:h-10 md:h-full md:flex flex-col justify-center font-bebas">
                <div class="hidden md:flex justify-end items-end md:space-x-6">
                    {#each navLinks as link}
                        <a href={link.link} class="font-medium tracking-wider text-lg text-blue-900 hover:text-red-700 active:text-red-800 transition ease-in-out duration-150">{link.name}</a>
                    {/each}
                </div>
            </nav>
        </div>
        <div class="block md:hidden px-4 sm:px-6 flex-grow ">
            <div class="h-full flex flex-col justify-center font-bebas">
                {#if !open}
                    <button on:click={() => opened()} class="block flex-grow rounded-md p-2 mr-8 inline-flex items-center justify-end text-gray-400 hover:text-gray-500 hover:cursor-pointer focus:outline-none md:hidden">
                        <span class="sr-only">Open Main Menu</span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                        </svg>
                    </button>
                {:else}
                    <button on:click={() => closed()} class="block flex-grow rounded-md p-2 mr-8 inline-flex items-center justify-end text-gray-400 hover:text-gray-500 hover:cursor-pointer focus:outline-none md:hidden">
                        <span class="sr-only">Close Main Menu</span>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                    </svg>

                    </button>
                {/if}
            </div>
        </div>
    </div>
    {#if open}
        <div class="relative md:hidden">
            <div class="absolute top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden">
                <div class="rounded-lg shadow-md bg-white ring-1 ring-black ring-opacity-5 overflow-hidden">
                    <div class="divide-y-2 divide-gray-50">
                        <div class="px-2 pt-2 pb-3">
                            {#each navLinks as link}
                                <a href={link.link} class="block px-3 py-2 rounded-md text-base font-medium text-blue-900 hover:text-red-800 hover:bg-gray-50">{link.name}</a>
                            {/each}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    {/if}
</div>