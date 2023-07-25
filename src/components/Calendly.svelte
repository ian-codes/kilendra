<script>
	import { onMount } from 'svelte';

	let calendlyWrapper;

	onMount(() => {
		Calendly.initInlineWidget({
			url: 'https://calendly.com/kilendra/15min?hide_landing_page_details=1&hide_gdpr_banner=1"',
			parentElement: calendlyWrapper
		});
	});
</script>

<div bind:this={calendlyWrapper} />

<svelte:head>
	<script
		type="text/javascript"
		src="https://assets.calendly.com/assets/external/widget.js"></script>
</svelte:head>

<section id="schedule" bind:this={calendlyWrapper} />

<style>
	section {
		display: block;
		max-width: 1000px;
		width: auto;
		z-index: 10;
		height: 800px;
		margin-top: -8em;
	}

	@media only screen and (max-width: 1000px) {
		section {
			height: 1200px;
		}
	}

	@media only screen and (max-width: 840px) {
		section {
			height: 1200px;
			margin: 1em;
		}
	}
</style>
