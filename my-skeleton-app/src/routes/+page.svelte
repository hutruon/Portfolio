<script>
	import ProjectCard from "../lib/components/ProjectCard.svelte";
	import image from "$lib/images/Close-up-shot-of-female-feet-isolated-on-transparent-background-PNG.png";
	let yellow = ["bang", "bang", "bang", "bang", "bang", "bang"];
</script>

<div class="container h-full mx-auto flex justify-center items-center">
	<div class="grid grid-cols-3">
		{#each yellow as id}
			<ProjectCard 
				imgSrc={image} 
				projectTitle={id} 
				descriptionSummary={"great Project"} 
				description={"lorum ipsum"} 
				projectOwner={"max zinzi"}
			/>
		{/each}
	</div>
</div>
