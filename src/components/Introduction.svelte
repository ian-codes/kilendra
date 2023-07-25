<script>
	import Incentive from './Incentive.svelte';
</script>

<section class="description">
	<p>
		Wir sind eine Digitale Marketing Agentur, die anhand modernen Methoden die Kundenakquise für Schweizer Unternehmen erleichtert und automatisiert.
	</p>
	<div class="design">
		<Incentive />
		<div class="ad-image image" />
	</div>
</section>

<style>
	section {
		font-size: var(--paragraph-fontsize);
		position: relative;
		transition: all 0.3s ease;
		overflow: hidden;
	}

	h2,
	p {
		padding: 0 1rem;
		font-size: 1.5em;
	}

	h2 {
		padding-top: 1rem;
	}

	.ad-image {
		position: relative;
		width: 100%;
		background-image: url('/assets/ads.webp');
		background-size: contain;
		background-position: center;
		background-repeat: no-repeat;
		filter: drop-shadow(5px 6px 3px rgba(0, 0, 0, 0.815)) hue-rotate(320deg);
		/* animation: hover 6s infinite; */
	}

	@keyframes hover {
		0% {
			transform: scale(1) translateY(-5px);
		}
		50% {
			transform: scale(1.01) translateY(5px);
		}
		100% {
			transform: scale(1) translateY(-5px);
		}
	}

	div {
		height: 400px;
		display: flex;
		justify-content: space-between;
	}

	@media only screen and (max-width: 840px) {
		section {
			overflow: visible;
		}
		p {
			font-size: 1em;
		}

		.ad-image {
			width: 100%;
			bottom: -3em;
			position: absolute;
			background-size: contain;
		}
	}
</style>
