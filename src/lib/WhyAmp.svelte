<script>
    let whyContent = [
        {
            title: 'Provide Jobs for American Workers',
            description: 'Purchasing more American made goods will in turn lead to more American manufacturing and more employment opportunities for our domestic workforce.'
        },
        {
            title: 'Superior Quality and Craftsmanship',
            description: "One thing you can be sure of is the attention to detail and pride that American manufacturers put into their products, you won't find this in many foreign pop-up shops."
        },
        {
            title: 'Better for the Environment',
            description: 'Because these products are made right here in our own backyards less transportation resources are spent getting them to their final destinations. This is good for us and good for the environment we live in.'
        },
        {
            title: 'Manufactured in Safe Working Conditions',
            description: 'Workplace safety policies and standards are always at the forefront of American manufacturing. Buying "sweat shop" goods from overseas only enables these outfits to continue to take advantage of their "employees".'
        },
        {
            title: 'Help Grow and Strengthen the US Economy',
            description: 'By having the top economy in the world we in turn attract more businesses to want to operate here because our people have more money to spend. The more money and jobs we send overseas the faster we will see a decrease in all of these benefits.'
        },
    ]
</script>


<div class="bg-blue-900 text-white mb-24 font-proxima">
    <div class="max-w-7xl mx-auto py-16 px-4 sm:px-6 lg:py-24 lg:px-8 lg:grid lg:grid-cols-3 lg:gap-x-8">
        <div class="px-4">
            <h3 class="text-2xl text-white uppercase font-bebas tracking-widest">Today more than ever it's important to support local American businesses so that we may all get through these upcoming economic uncertainties.</h3>
            <p class="mt-4 text-lg text-gray-200">By being proactive and making an effort to buy American whenever possible we give ourselves and the economy the best opportunity to survive and thrive.</p>
        </div>
        <div class="mt-12 lg:mt-0 lg:col-span-2">
            <div class="space-y-10 sm:space-y-0 sm:grid sm:grid-cols-2 sm:grid-rows-3 sm:grid-flow-col sm:gap-x-6 sm:gap-y-10 lg:gap-x-8">
                {#each whyContent as content}
                    <div class="flex">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="flex-shrink-0 h-6 w-6 text-red-700">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12.75l6 6 9-13.5" />
                        </svg>

                        <div class="ml-3">
                            <h1 class="text-lg leading-6 font-medium text-white">{content.title}</h1>
                            <p class="mt-2 text-base text-gray-200">{content.description}</p>
                        </div>
                    </div>
                {/each}
            </div>
        </div>
    </div>
</div>