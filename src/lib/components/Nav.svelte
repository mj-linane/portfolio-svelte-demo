<!-- Nav.svelte -->
<script>
	export let menuItems = [
		{ label: 'Home', href: '/' },
		{ label: 'Tribute', href: '/tribute' },
		{ label: 'Form', href: '/form' },
		{ label: 'Sales', href: '/sales' }
	];
</script>

<nav>
	<ul>
		{#each menuItems as item}
			<li>
				<a href={item.href}>{item.label}</a>
			</li>
		{/each}
	</ul>
</nav>

<style>
	nav {
		display: flex;
		justify-content: flex-end;
	}

	ul {
		display: flex;
		list-style: none;
		margin: 0;
		padding: 0;
	}

	li {
		margin-left: 1rem;
	}

	a {
		color: #333;
		text-decoration: none;
	}
</style>
