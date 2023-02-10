<!-- ⚙️ Imports + Logic (Sub-section 2) -->
<script>
	import Heading from "../../../../lib/typography/Heading.svelte";
	import Paragraph from "../../../../lib/typography/Paragraph.svelte";

	// Define URL path to reference in 'src' values.
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 2) -->
<div>
	<!-- 📐 Mini-section 3 -->
	<div>
		<!-- Title -->
		<Heading size={"h2"} color={"light"} text={"Javascript"} />

		<!-- Description -->
		<Paragraph
			size={"small"}
			color={"light"}
			text={"Statically generated pages are brought to life with client-side JavaScript libraries and frameworks, such as Algolia and Next.js."}
		/>
	</div>

	<!-- 📐 Mini-section 4 -->
	<div>
		<!-- Graphic -->
		<img
			src="{src}{`retro-computer.svg`}"
			alt="An old retroesque computer monitor displaying some lines of code on a black background"
		/>
	</div>
</div>

<!-- 🎨 Styles (Sub-section 2) -->
<style>
</style>
