<!-- ⚙️ Imports + Logic (Sub-section 3) -->
<script>
	// Define URL path to reference in 'src' values
	let src = "/img/logos/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 3) -->
<div>
	<!-- 💡IDEA: The code to render the 8 logos still seems a bit DRY. Logos can be more modularized/optimized by making them .svelte components with the help of their bightness/opacity differences -->

	<!-- Full-white Next.js Logo -->
	<img
		src="{src}{`nextjs-logo.svg`}"
		alt="A white logo of Next.js on a dark background"
		class="nextjs"
	/>

	<!-- Full-white React Logo -->
	<img
		src="{src}{`react-logo.svg`}"
		alt="A white logo of React on a dark background"
	/>

	<!-- Full-white Next.js Logo -->
	<img
		src="{src}{`nextjs-logo.svg`}"
		alt="A white logo of Next.js on a dark background"
	/>

	<!-- Full-white React Logo -->
	<img
		src="{src}{`react-logo.svg`}"
		alt="A white logo of React on a dark background"
	/>

	<!-- Slightly-dimmed Svelte Logo -->
	<img
		src="{src}{`svelte-logo-dimmed.svg`}"
		alt="A slightly-dimmed white logo of Svelte on a dark background"
	/>

	<!-- Slightly-dimmed Vue.js Logo -->
	<img
		src="{src}{`vuejs-logo-dimmed.svg`}"
		alt="A slightly-dimmed white logo of Vue.js on a dark background"
	/>

	<!-- Quite-faint React Logo -->
	<img
		src="{src}{`react-logo-faint.svg`}"
		alt="A very faint white logo of React on a dark background"
	/>

	<!-- Quite-faint Svelte Logo -->
	<img
		src="{src}{`svelte-logo-faint.svg`}"
		alt="A very faint white logo of Svelte on a dark background"
	/>
</div>

<!-- 🎨 Styles (Sub-section 3) -->
<style>
</style>
