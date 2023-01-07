<script>
	import Hero from "$lib/Hero.svelte";

</script>

<svelte:head>
	<title>Contact</title>
</svelte:head>

<Hero heroImage="/images/ampHero.jpeg" />
<div class="px-4 sm:px-10 lg:px-12 text-center lg:max-w-5xl mx-auto mb-8 pb-20 lg:pb-24 ">
    <h1 class="font-bebas text-3xl uppercase tracking-widest text-blue-900 mb-8 lg:mb-18">Contact American Made Products</h1>
    <div class="font-proxima text-lg tracking-wide text-gray-700 leading-8 pb-8">Want to see a brand listed that's not already here? Is something on the site not working? Drop us a line below with this or any other info and we will get back to you asap.</div>
    <div class="mt-3 sm:mt-5 clear-both px-12 max-w-xl mx-auto">
        <h3 class="text-lg leading-6 tracking-wider font-medium text-blue-900 font-bebas uppercase pt-6 pb-2">Contact Us</h3>
        <div class="mt-2">
            <form method="post">
                <input type="hidden" name="form-name">
                <div class="grid grid-cols-12">
                    <div class="col-span-12 mt-2">
                        <label for="name" class="block text-sm font-bold text-gray-700 text-left">Name*</label>
                        <div class="mt-1">
                            <input type="text" name="name" id="name" required class="p-2 shadow-sm focus:ring-yellow-500 focus:border-red-700 block w-full sm:text-sm border-blue-900 border-2">
                        </div>
                    </div>
                    <div class="col-span-12 mt-2">
                        <label for="email" class="block text-sm font-bold text-gray-700 text-left">Email*</label>
                        <div class="mt-1">
                            <input type="email" name="email" id="email" required autocomplete="email" class="p-2 shadow-sm focus:ring-yellow-500 focus:border-red-700 block w-full sm:text-sm border-blue-900 border-2">
                        </div>
                    </div>
                    <div class="col-span-12 mt-2">
                        <label for="subject" class="block text-sm font-bold text-gray-700 text-left">Subject</label>
                        <div class="mt-1">
                            <select name="subject" id="subject" required autocomplete="subject" class="block p-2 shadow-sm focus:ring-yellow-500 focus:border-red-700 block w-full sm:text-sm border-blue-900 border-2">
                                <option value="Become Featured">Become a Featured Product</option>
                                <option value="Add Product">Add a Product</option>
                                <option value="Information Request">Information Request</option>
                                <option value="Website Issue">Website Issue</option>
                                <option value="Other">Other</option>

                        </div>
                    </div>
                    <div class="col-span-12 mt-2">
                        <label for="message" class="block text-sm font-bold text-gray-700 text-left">Message*</label>
                        <div class="mt-1">
                            <textarea name="message" id="message" required class="p-2 shadow-sm focus:ring-yellow-500 focus:border-red-700 block w-full sm:text-sm border-blue-900 border-2"></textarea>
                        </div>
                    </div>
                    <div class="col-span-12 mt-2">
                        <button type="submit" class="mt-4 px-12 py-2 border-2 border-blue-900 font-bebas tracking-widest uppercase text-blue-900 hover:border-red-700 hover:text-red-700 transition ease-in-out duration-150 mx-auto">Submit</button>
                    </div>
                </div>
            </form>
        </div>
    </div>
</div>