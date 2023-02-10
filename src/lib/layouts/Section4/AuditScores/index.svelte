<!-- ⚙️ Imports + Logic (Sub-section 7) -->
<script>
	import Heading from "../../../../lib/typography/Heading.svelte";
	import Paragraph from "../../../../lib/typography/Paragraph.svelte";

	// Define URL path to reference in 'src' values
	let src = "/img/graphics/";

	// 🪧 Better to do use an 'img' tag rather than abstracting it into an 'Image.svelte' component as the 'img' tag would get generated at runtime and in order to style it locally below, the ':global()' modifier would need to be used, thus ruining the fun that writing CSS can be :P

	// 🪧 A class can be added as a prop to that hypothetical 'Image.svelte' component but wherever that component would be used without any local styles added, it would just result in a non-necessary abstraction, thus making web development more complicated than it already is :P
</script>

<!-- 🧱 Structure (Sub-section 7) -->
<div id="sub-section-7">
	<!-- 📐 Mini-section 11 -->
	<div>
		<!-- Title -->
		<Heading size={"h3"} color={"pastel-green"} text={"Top Audit Scores"} />

		<!-- 4 Score Circles -->
		<div id="score-list">
			<img
				src="{src}{`score-with-glowing-ring.svg`}"
				alt="The number 100 mentioned in bright glowing pastel green with a similar-looking glowing ring around it"
				class="score"
			/>
			<img
				src="{src}{`score-with-glowing-ring.svg`}"
				alt="The number 100 mentioned in bright glowing pastel green with a similar-looking glowing ring around it"
				class="score"
			/>
			<img
				src="{src}{`score-with-glowing-ring.svg`}"
				alt="The number 100 mentioned in bright glowing pastel green with a similar-looking but non-glowing ring around it"
				class="score"
			/>
			<img
				src="{src}{`score-with-glowing-ring.svg`}"
				alt="The number 100 mentioned in bright glowing pastel green with a similar-looking glowing ring around it"
				class="score"
			/>
		</div>
	</div>

	<!-- 📐 Mini-section 12 -->
	<div>
		<!-- Explainer -->
		<Paragraph
			size={"big"}
			color={"grey"}
			text={"Search engines, business stakeholders, and end-users gauge a website’s value using metric tools like Google Lighthouse, which measures site performance, SEO, and accessibility."}
		/>

		<Paragraph
			size={"big"}
			color={"grey"}
			text={"Performance is one of the most difficult scores to get to 100. This is especially true in a time when users demand JavaScript-heavy, highly-interactive web experiences."}
		/>

		<Paragraph
			size={"big"}
			color={"grey"}
			text={"A Jamstack website, delivering SEO-friendly, lean & clean HTML in milliseconds, promises higher search-engine ranking and a more positive, responsive end-user experience."}
		/>
	</div>
</div>

<!-- 🎨 Styles (Sub-section 7) -->
<style>
	#sub-section-7 {
		background: linear-gradient(
			25.39deg,
			rgba(255, 255, 255, 0.024) 18.54%,
			rgba(123, 245, 93, 0.108) 62.25%
		);
		border-radius: 68px;
		backdrop-filter: blur(60px);
		mix-blend-mode: normal;
	}

	#score-list {
		display: flex;
		flex-direction: row;
	}

	.score {
		width: 212px;
		height: 212px;
	}

	/* Using the ':global()' modifier as the 'heading' class is being applied to the 'Heading' component at runtime */
	.score :global(.heading) {
		text-shadow: 0px 0px 12px #53fb2a, 0px 0px 42px #e9e11f,
			0px 0px 61px #53fb2a;
	}
</style>
