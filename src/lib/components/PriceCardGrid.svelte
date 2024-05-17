<script>
	import PriceCard from '$lib/components/PriceCard.svelte';
	export let priceTiers = [];
</script>

<section class="price-cards-container">
	<div class="price-card-row">
		{#if priceTiers.length > 0}
			{#each priceTiers as { priceTier, price, features }}
				<PriceCard {priceTier} {price} {features} />
			{/each}
		{/if}
	</div>
</section>

<style>
	.price-cards-container {
		background-color: green;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 4rem;
	}
	.price-card-row {
		max-width: 80%;
		border-color: red;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: space-between;
		gap: 20px;
	}
</style>
