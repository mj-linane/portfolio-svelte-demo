<script>
	export let title = "MJ Linane's Portfolio";
</script>

<div class="hero">
	<div class="hero-content">
		<h1>{title}</h1>
	</div>
</div>

<style>
	.hero {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		min-height: 100vh;
		width: 100%;
		background-size: cover;
		background-position: center;
		position: relative;
		background: rgb(34, 0, 136);
		background: linear-gradient(45deg, rgba(34, 0, 136, 1) 0%, rgba(255, 0, 241, 1) 100%);
	}

	.hero::before {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: 1;
	}

	.hero-content {
		text-align: center;
		color: white;
		z-index: 2;
		/* padding: 1rem; */
	}

	h1 {
		font-size: 4rem;
		margin-bottom: 1rem;
	}
</style>
