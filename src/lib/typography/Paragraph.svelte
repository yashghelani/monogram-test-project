<script>
	export let size, color, text;
</script>

<svelte:element this={size} class={color}>{text}</svelte:element>

<style>
	/* Define size-based properties */

	p {
		font-style: normal;
	}

	.small {
		font-weight: 300;
		font-size: 18px;
		line-height: 195.5%;
		letter-spacing: 0.005em;
	}

	.medium,
	.big {
		font-weight: 400;
		line-height: 162%;
	}

	.medium {
		font-size: 24px;
	}

	.big {
		font-size: 26px;
	}

	/* ////////// */

	/* Define color-based properties */

	.light {
		color: #ffffff;
	}

	.dark {
		color: #414141;
	}

	.dark-alt {
		color: #757575;
	}

	.grey {
		color: #c7c7c7;
	}
</style>
