<!-- ⚙️ Imports + Logic (Sub-section 6) -->
<script>
	// Define URL path to reference in 'src' values
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 6) -->
<div>
	<!-- 📐 Mini-section 9 -->
	<div>
		<!-- Toppled Blocks -->
		<img src="{src}{`single-toppled-block-blue.svg`}" alt="" />
		<img src="{src}{`single-toppled-block-red.svg`}" alt="" />
		<img src="{src}{`single-toppled-block-yellow.svg`}" alt="" />
	</div>

	<!-- 📐 Mini-section 10 -->
	<div>
		<!-- Wall of Blocks -->
		<img src="{src}{`wall-of-blocks-cropped.svg`}" alt="" />
	</div>
</div>

<!-- 🎨 Styles (Sub-section 6) -->
<style>
</style>
