<script>
	import Incentive from './Incentive.svelte';
</script>

<section class="description">
	<h2>unser Kompetenzbereich</h2>
	<p>
		Bei Kilendra fokussieren wir uns auf ein Ziel: <b>Kundenakquise</b>.
		Mit unserem tiefgehenden Fachwissen in den Bereichen Digital Marketing, Soziale Medien, Lead-Generierung, Lead-Nurturing und Automatisierung helfen wir Ihnen, die Kundengewinnung möglichst effizient und mühelos zu gestalten, um somit mehr Zeit und Energie für das Wesentliche zu haben - Ihr Unternehmen.
	</p>
	<div>
		<Incentive />
		<div class="target-image image" />
	</div>
</section>

<style>
	section {
		overflow: hidden;
		font-size: var(--paragraph-fontsize);
		position: relative;
		transition: all 0.3s ease;
	}

	h2,
	p {
		padding: 0 1rem;
	}

	h2 {
		padding-top: 1rem;
	}

	div {
		height: 450px;
		display: flex;
		justify-content: space-between;
	}

	.target-image {
		position: relative;
		width: 100%;
		background-image: url('/assets/target.webp');
		background-size: 70%;
		background-position: center;
		background-repeat: no-repeat;
		filter: drop-shadow(5px 6px 3px rgba(0, 0, 0, 0.815)) hue-rotate(320deg);
		z-index: -9;
	}

	@media only screen and (max-width: 840px) {
		section {
			overflow: visible;
		}

		.target-image {
			width: 100%;
			position: absolute;
			background-size: contain;
			bottom: -3em;
		}
	}
</style>
