<script>
import LinkCard from '../components/LinkCard.svelte';
	$: list = [
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
<div class="flex mb-4 flex-wrap -mx-2 mb-4">

{#each list as item}
	<LinkCard {item}></LinkCard>
{/each}
</div>