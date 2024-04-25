<script>
	import ProjectCard from '$lib/components/ProjectCard.svelte';
	export let itemsPerRow = 3;
	export let projects = [
		{
			name: 'Project 1',
			description: 'This is a description of project 1',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		},
		{
			name: 'Project 2',
			description: 'This is a description of project 2',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		},
		{
			name: 'Project 3',
			description: 'This is a description of project 3',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		},
		{
			name: 'Project 4',
			description: 'This is a description of project 4',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		},
		{
			name: 'Project 5',
			description: 'This is a description of project 5',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		},
		{
			name: 'Project 6',
			description: 'This is a description of project 6',
			image: 'https://via.placeholder.com/300',
			link: 'https://google.com'
		}
	];
</script>

<section style="display: grid; grid-template-columns: repeat({itemsPerRow}, 1fr); gap: 1rem;">
	{#each projects as project}
		<ProjectCard
			name={project.name}
			description={project.description}
			image={project.image}
			link={project.link}
		/>
	{/each}
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}
</style>
