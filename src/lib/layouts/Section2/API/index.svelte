<!-- ⚙️ Imports + Logic (Sub-section 4) -->
<script>
	import Heading from "../../../../lib/typography/Heading.svelte";
	import Paragraph from "../../../../lib/typography/Paragraph.svelte";

	// Define URL path to reference in 'src' values
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 4) -->
<div>
	<!-- 📐 Mini-section 5 -->
	<div>
		<!-- Title -->
		<Heading size={"h2"} color={"light"} text={"API"} />

		<!-- Description -->
		<Paragraph
			size={"medium"}
			color={"light"}
			text={"At build time, a Jamstack website uses data from one or more APIs to generate markup. These APIs can be a headless CMS like Prismic, a database like Supabase, or even a local JSON file!"}
		/>
	</div>

	<!-- 📐 Mini-section 6 -->
	<div>
		<!-- Graphic -->
		<img
			src="{src}{`glowing-logo-circle.svg`}"
			alt="A glowing circle with logos of Prismic and Supabase wrapped around it"
		/>
	</div>
</div>

<!-- 🎨 Styles (Sub-section 4) -->
<style>
</style>
