<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-5 mt-5">
		<h1>Welcome to my New Media Portfolio</h1>
		<h3>Im a <span class="rainbow">Computer Science</span> student with a background in Web Development</h3>
		<hr/>
		<h4>Start by exploring:</h4>
		<ul>
			<li><h5><a class="underline" href="/project-a">PhotoShop Project</a></h5></li>
			<li><h5><a href="/project-b"><span class="underline">Website Project</span> (this one)</a></h5></li>
			<li><h5><a href="/project-c"><span class="underline">Video Project</span> (tbd)</a></h5></li>
		</ul>
	</div>
</div>


<style>
	.rainbow {
		background-image: linear-gradient(90deg, #f79533, #f37055, #ef4e7b, #a166ab, #5073b8, #1098ad, #07b39b, #6fba82, #b1c471, #fde725);
		background-size: 200% 200%;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		animation: rainbow 5s linear infinite;
	}

	@keyframes rainbow {
		0% {
			background-position: 0% 82%
		}
		50% {
			background-position: 100% 19%
		}
		100% {
			background-position: 0% 82%
		}
	}
</style>