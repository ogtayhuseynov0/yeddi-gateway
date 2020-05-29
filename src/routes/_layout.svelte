<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>
<!-- <Nav {segment}/> -->
<!-- 
<main>
	<slot></slot>
</main> -->
<div class="h-screen flex flex-col">
	<div class=" h-12 min-h-12 bg-gray-900 flex text-gray-200  items-center px-6">
	<button>
	<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-menu"><path d="M3 12h18M3 6h18M3 18h18"/></svg>
	</button>
		<span class="text-lg font-semibold antialiased ml-6">Yeddi Link Gateway</span>
	</div>
	<div class="flex h-screen">
		<div class=" w-64 min-w-64 bg-gray-900 flex"> 
			<Nav segment={segment}></Nav>
		</div>
		<div class="flex-grow bg-gray-100 p-4">
			<slot></slot>
		</div>
	</div>
</div>