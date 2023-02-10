<!-- ⚙️ Imports + Logic (Full page) -->
<script>
	import Section1 from "./lib/layouts/Section1/index.svelte";
	import Section2 from "./lib/layouts/Section2/index.svelte";
	import Section3 from "./lib/layouts/Section3/index.svelte";
	import Section4 from "./lib/layouts/Section4/index.svelte";
</script>

<!-- 🧱 Structure (Full page) -->
<main>
	<!-- Jamstack101 + JavaScript -->
	<Section1 />

	<!-- FillerLogos + API -->
	<Section2 />

	<!-- Markup + FillerBlocks -->
	<Section3 />

	<!-- AuditScores + Footer -->
	<Section4 />
</main>

<!-- 🎨 Styles (Full page) -->
<style>
	main {
		display: flex;
		flex-direction: column;
		row-gap: 150px;
	}
</style>
