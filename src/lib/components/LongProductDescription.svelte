<script>
	export let productHeadline = 'Product Description';
</script>

<section class="long-product-description">
	<h2>{productHeadline}</h2>
	<slot />
</section>

<style>
	section {
		padding: 2rem 3rem;
	}

	h2 {
		text-align: center;
		font-size: 3rem;
	}
</style>
