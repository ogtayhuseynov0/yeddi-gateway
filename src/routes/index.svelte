<script>
import LinkCard from '../components/LinkCard.svelte';
	$: list = [
		{
			name: 'Guraba',
			img: 'guraba.PNG',
			link: 'https://guraba.be/'
		},
		{
			name: 'GameMatcher',
			img: 'game.PNG',
			link: 'https://gamematcher.yeddi.ml/'
		},
		{
			name: 'Vote',
			img: 'vote.PNG',
			link: 'https://vote.yeddi.ml/'
		},
		{
			name: 'Alpr',
			img: 'alpr.PNG',
			link: 'https://alpr.yeddi.ml/'
		},
		{
			name: 'OLinkDB',
			img: 'olink.PNG',
			link: 'https://olinkdb.yeddi.ml/'
		}
	];
</script>

<style>

</style>

<svelte:head>
	<title>Yeddi GateWay</title>
</svelte:head>
<div class="text-center mb-4 font-medium">
<div class="bg-green-100 border-l-4 border-green-500 text-green-700 p-4" role="alert">
  <p class="font-bold">Complete Projects</p>
</div>
</div>
<div class="flex mb-4 flex-wrap -mx-2 mb-4">

{#each list as item}
	<LinkCard {item}></LinkCard>
{/each}
</div>