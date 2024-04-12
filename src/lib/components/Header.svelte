<!-- Header.svelte -->
<script>
	import Nav from './Nav.svelte';

	export let siteName = 'My Portfolio';
	export let logoSrc = '/logo.svg' //static;
</script>

<header>
	<div class="logo">
		<img src={logoSrc} alt={siteName} />
		<span>{siteName}</span>
	</div>
	<Nav />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem;
		background-color: #f5f5f5;
	}

	.logo {
		display: flex;
		align-items: center;
	}

	.logo img {
		height: 40px;
		margin-right: 0.5rem;
	}

	.logo span {
		font-size: 1.5rem;
		font-weight: bold;
	}
</style>
