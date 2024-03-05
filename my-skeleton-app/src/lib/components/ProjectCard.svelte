<script>
	import { Avatar } from '@skeletonlabs/skeleton';
	export let projectTitle;
	export let descriptionSummary;
	export let description;
	export let projectOwner;
	export let imgSrc;
</script>


	<a class="card card-hover overflow-hidden variant-filled-primary m-4" href="/elements/cards">
		<header>
			<img src={imgSrc} class="bg-black/50 w-full aspect-[21/9]" alt="Post" />
		</header>
		<div class="p-4 space-y-4">
			<h6 class="h6" data-toc-ignore>{projectTitle}</h6>
			<h3 class="h3" data-toc-ignore>{descriptionSummary}</h3>
			<article>
				<p>
					{description}
				</p>
			</article>
		</div>
		<hr class="opacity-50" />
		<footer class="p-4 flex justify-start items-center space-x-4">
			<Avatar width="w-8" />
			<div class="flex-auto flex justify-between items-center">
				<h6 class="font-bold" data-toc-ignore>{projectOwner}</h6>
				<small>On {new Date().toLocaleDateString()}</small>
			</div>
		</footer>
	</a>
