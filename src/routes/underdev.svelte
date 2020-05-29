<script>
import LinkCard from '../components/LinkCard.svelte';
	$: list = [
         {
			name: 'Auction',
			img: 'auc.PNG',
			link: 'http://auction.yeddi.ml/'
		},
        {
			name: 'Araz Watches',
			img: 'araz.PNG',
			link: 'https://araz.yeddi.ml/'
        },
		{
            name: 'Nurlan Isayev',
			img: 'nis.PNG',
			link: 'http://live.yeddi.ml/'
		},
                                {
                                    name: 'Telegram bot Dashboard',
                                    img: 'az.png',
                                    link: 'none'
                                },
	];
</script>

<style>

</style>

<svelte:head>
	<title>Yeddi GateWay</title>
</svelte:head>
<div class="text-center mb-4 font-medium">
<div class="bg-orange-100 border-l-4 border-orange-500 text-orange-700 p-4" role="alert">
  <p class="font-bold">Under Development Projects</p>
</div>
</div>
<div class="flex mb-4 flex-wrap -mx-2 justify-center mb-4 ">

{#each list as item}
	<LinkCard {item}></LinkCard>
{/each}
</div>