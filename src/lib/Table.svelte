<script>
    export let title = '';
    export let description = '';
    export let name = '';
    export let link = '';
</script>
<div class="text-center">
    <h2 class="text-3xl tracking-widest font-base text-blue-900 sm:text-4xl font-bebas tracking-widest">{title}</h2>
    <p class="mt-3 max-w-2xl mx-auto text-xl text-gray-500 sm:mt-4">{description}</p>
</div>
<div class="shadow-lg overflow-hidden border-b border-gray-200 sm:rounded-lg mt-12">
    <table class="min-w-full divide-y divide-gray-200">
        <thead class="bg-gray-50">
            <tr>
                <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Name</th>
                <th scope="col" class="relative px-6 py-3">
                    <span class="sr-only">View</span>
                </th>
            </tr>
        </thead>
        <tbody>
            <tr class="bg-white hover:bg-gray-100 hover:cursor-pointer">
                <td class="whitespace-nowrap text-sm font-medium text-gray-900">
                    <a href={link} class="text-blue-900 hover:text-red-700">
                        <div class="w-full px-6 py-2">{name}</div>
                    </a>
                </td>
                <td class="px-6 py-2 whitespace-nowrap text-right text-sm font-medium">
                    <a href={link} class="text-blue-900 hover:text-red-700">
                        <div class="w-full px-6 py-2">View</div>
                    </a>
                </td>
            </tr>
        </tbody>
    </table>
</div>