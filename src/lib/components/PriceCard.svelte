<script>
	export let priceTier;
	export let price;
	export let features;
</script>

<div class="price-card">
	<div class="card-title">
		<h2>{priceTier}</h2>
		<h3>${price}</h3>
	</div>
	<div class="card-content">
		<ul>
			{#each features as feature}
				<li>{feature}</li>
			{/each}
		</ul>
	</div>
</div>

<style>
	.price-card {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		border: 1px solid #ccc;
		border-radius: 8px;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
	}

	.card-title {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin-bottom: 1rem;
	}

	h2 {
		font-size: 1.5rem;
		margin-bottom: 0.5rem;
	}

	h3 {
		font-size: 1.25rem;
		margin-bottom: 1rem;
	}

	.card-content {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		font-size: 1rem;
		margin-bottom: 0.5rem;
	}
</style>
