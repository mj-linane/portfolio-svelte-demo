<!-- Single ProjectCard -->
<script>
	export let name;
	export let description;
	export let image;
	export let link;
</script>

<div class="project-card">
	<a href={link} target="_blank">
		<img src={image} alt={name} />
		<h2>{name}</h2>
		<p>{description}</p>
		<img src={image} alt={name} />
		<h2>{name}</h2>
		<p>{description}</p>
	</a>
</div>

<style>
	.project-card {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 1rem;
		border: 1px solid #ccc;
		border-radius: 8px;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
	}

	img {
		width: 100%;
		border-radius: 8px;
		margin-bottom: 1rem;
	}

	h2 {
		font-size: 1.5rem;
		margin-bottom: 0.5rem;
	}

	p {
		font-size: 1rem;
		margin-bottom: 1rem;
	}
</style>
