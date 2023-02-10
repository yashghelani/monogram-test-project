<!-- ⚙️ Imports + Logic (Sub-section 5) -->
<script>
	import Heading from "../../../../lib/typography/Heading.svelte";
	import Paragraph from "../../../../lib/typography/Paragraph.svelte";

	// Define URL path to reference in 'src' values
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 5) -->
<div>
	<!-- 📐 Mini-section 7 -->
	<div>
		<!-- Title -->
		<Heading size={"h2"} color={"dark"} text={"Markup"} />

		<!-- Description -->
		<Paragraph
			size={"medium"}
			color={"dark"}
			text={"When ready for deployment, a static-site generator such as Astro or Next.js is used to compile the website. The end result is a collection of pre-rendered HTML pages that can be delivered lightning-fast over a CDN like Vercel’s Edge Network."}
		/>
	</div>

	<!-- 📐 Mini-section 8 -->
	<div>
		<!-- 4 Vertical Bars Graphic -->
		<img
			src="{src}{`vertical-bars-section-2.png`}"
			alt="A graphical representation of 4 vertical bars. Two short and opaque ones on the front, and two longer ones with a stack of tiny LEGO bricks filling them"
		/>
	</div>
</div>

<!-- 🎨 Styles (Sub-section 5) -->
<style>
</style>
