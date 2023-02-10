<!-- ⚙️ Imports + Logic (Sub-section 1) -->
<script>
	import Heading from "../../../../lib/typography/Heading.svelte";
	import Paragraph from "../../../../lib/typography/Paragraph.svelte";

	// Define URL path to reference in 'src' values.
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 1) -->
<div>
	<!-- 📐 Mini-section 1 -->
	<div>
		<!-- Title -->
		<Heading size={"h1"} color={"dark-alt"} text={"Jamstack 101"} />

		<!-- Description -->
		<Paragraph
			size={"small"}
			color={"dark-alt"}
			text={"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Arcu augue massa, tincidunt proin nunc viverra tristique tempor, ipsum. At lectus vel pretium tempor ut dui vivamus sit."}
		/>

		<!-- Mouse and Squiggly Arrow -->
		<img
			src="{src}{`mouse-with-squiggly-arrow.svg`}"
			alt="A tiny computer mouse icon with a dotted squiggly path going towards the bottom of the screen and ends with a lined arrow head"
		/>
	</div>

	<!-- 📐 Mini-section 2 -->
	<div>
		<!-- 4 Vertical Bars Graphic -->
		<img
			src="{src}{`vertical-bars-section-1.png`}"
			alt="A graphical representation of 4 vertical bars. Two short and opaque ones on the front, and two longer ones with a warm-colored wavy illustration filling them"
		/>
	</div>
</div>

<!-- 🎨 Styles (Sub-section 1) -->
<style>
</style>
