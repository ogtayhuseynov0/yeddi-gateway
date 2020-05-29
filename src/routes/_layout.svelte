<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
	$: drawer = false;
</script>
<!-- <Nav {segment}/> -->
<!-- 
<main>
	<slot></slot>
</main> -->
<div class="h-screen flex flex-col">
	<div class=" h-12 min-h-12 bg-gray-900 flex text-gray-200  items-center px-6 flex-none">
	<button on:click="{() => drawer = !drawer}">
	<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-menu"><path d="M3 12h18M3 6h18M3 18h18"/></svg>
	</button>
		<span class="text-lg font-semibold antialiased ml-6">Yeddi Link Gateway</span>
	</div>
	<div class="flex h-screen">
	<!-- {#if drawer} -->
	<div class="hidden sm:w-64 sm:flex flex-no-shrink flex-none bg-gray-900 flex" class:hidden={drawer} class:sm:flex={!drawer} class:sm:w-64={!drawer}> 
			<Nav segment={segment} ></Nav>
		</div>
	<!-- {/if} -->
		
		<div class="flex-grow bg-gray-100 p-4 overflow-hidden overflow-y-scroll">
			<slot></slot>
		</div>
	</div>
</div>