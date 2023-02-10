<script>
	export let size, color, text;
</script>

<svelte:element this={size} class={color + ` heading`}>{text}</svelte:element>

<style>
	/* Define size-based properties */

	h1,
	h2,
	h3 {
		font-style: normal;
		font-weight: 900;
		letter-spacing: -0.039em;
		text-transform: lowercase;
	}

	h1,
	h2 {
		font-size: 133px;
		line-height: 115%;
	}

	h3,
	h4 {
		line-height: auto;
		text-align: center;
	}

	h3 {
		font-size: 76px;
	}

	h4 {
		font-size: 63px;
	}

	/* ////////// */

	/* Define color-based properties */

	.light {
		color: #ffffff;
	}

	.dark {
		color: #151515;
	}

	.pastel-green {
		color: #efffe2;
	}
</style>
