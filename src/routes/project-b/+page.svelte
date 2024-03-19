<script>
  import svelteLogo from '$lib/assets/svelte.png';
  import tailwindLogo from '$lib/assets/tailwindcss.png';
  import sveltekitLogo from '$lib/assets/sveltekit.png';
</script>


<main class="flex justify-center align-center">
  <div class="card w-1/3 p-2 mt-4">
    <h2 class="my-2">Website Development</h2>
    <p class="my-2">For this website development project, I used technologies that I have used in my professional career. To create this site, I used a frontend framework called Svelte and Sveltekit,
      which allowed me to write HTML like code while being able to components, and javascript within my pages. I used TailwindCSS for writing inline CSS for styling.</p>
    <hr class="my-1"/>
    <div class="inline-flex justify-center align-center m-2 my-4 gap-4">
      <img src={sveltekitLogo} alt="Sveltekit Logo" class="h-1/2 w-1/2"/>
      <img src={tailwindLogo} alt="Tailwind Logo" class="w-1/6"/>
    </div>

  </div>
</main>

