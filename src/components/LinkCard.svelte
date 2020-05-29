<script>
export let item;
</script>

<div class="w-full justify-center flex md:w-1/2 lg:w-1/3 px-2 mb-2">
<div class="max-w-sm rounded overflow-hidden shadow-lg">
    <!-- <div class="relative bg-red-500 "> -->
     <img class="w-full object-cover  " src="{item.img}" alt="GameMatcher screenshot">
    <!-- </div> -->
   

	<div class="px-6 py-4">
		<div class="font-bold text-xl text-center text-gray-800">{item.name}</div>
	
	</div>
	<div class="px-6 py-4">
    {#if item.link === 'none'}
    	<div class="p-2 bg-red-300 items-center text-red-600 leading-none  flex justify-between rounded-full " role="alert">
		<span class="flex rounded-full bg-red-400 uppercase px-2 py-1 text-xs font-bold mr-3">Offline</span>
		<span class="font-semibold mr-2 text-left flex items-center">Can't Open &nbsp;
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-circle"><circle cx="12" cy="12" r="10"/><path d="M15 9l-6 6M9 9l6 6"/></svg></span>
		</div>
    {:else}
	<div class="p-2 bg-green-300 items-center text-green-600 leading-none  flex justify-between rounded-full " role="alert">
		<span class="flex rounded-full bg-green-400 uppercase px-2 py-1 text-xs font-bold mr-3">Online</span>
		<a href="{item.link}" target="_blank">
		<span class="font-semibold mr-2 text-left flex items-center">Open &nbsp;
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24"
		fill="none" stroke="currentColor"
		stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-external-link"><path d="M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6M15 3h6v6M10 14L21 3"/></svg>
		</span>
		</a>
		</div>
    {/if}
 </div>
	</div>
</div>