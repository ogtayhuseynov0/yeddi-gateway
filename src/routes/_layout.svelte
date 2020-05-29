<script>
	// import Nav from '../components/Nav.svelte';

	// export let segment;
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
			<ul class="flex flex-col w-full font-medium">
				<li class="flex mx-2">
					<a class=" flex text-center w-full block rounded py-2 px-4 text-gray-200 hover:bg-gray-800" href="/">
					<svg xmlns="http://www.w3.org/2000/svg"
					 width="24" height="24"
					  fill="none"
					   stroke="currentColor" 
					   stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
					    class=" feather feather-check-circle"><path d="M22 11.08V12a10 10 0 11-5.93-9.14"/><path d="M22 4L12 14.01l-3-3"/></svg>
						<span class="ml-6">Complete</span>
					</a>
				</li>
				<li class="flex mx-2">
					<a class=" flex text-center w-full block rounded py-2 px-4 text-gray-200 hover:bg-gray-800"
					 href="/underdev">
					<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-code"><path d="M16 18l6-6-6-6M8 6l-6 6 6 6"/></svg>
						<span class="ml-6">Under Dev</span>
					</a>
				</li>
			</ul>
		</div>
		<div class="flex-grow bg-gray-100 p-4">
			<slot></slot>
		</div>
	</div>
</div>