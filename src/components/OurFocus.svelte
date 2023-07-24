<script>
	import Incentive from './Incentive.svelte';
</script>

<section class="description" id="how-we-work">
	<h2>VORGEHENSWEISE</h2>
	<!-- 	<p>Here's how we operate</p> -->
	<ul>
		<li>
			<span>&#x2714;</span>
			<p>Wir analysieren Ihr Geschäft.</p>
		</li>
		<li>
			<span>&#x2714;</span>
			<p>Wir erstellen einen Plan, welcher der Vision Ihrer Geschäftsidentität entspricht.</p>
		</li>
		<li>
			<span>&#x2714;</span>
			<p>Wir erstellen und betreiben Ihre Werbekampagnen auf der Grundlage einer ganzheitlichen Betrachtung Ihres Unternehmens.</p>
		</li>
		<li>
			<span> &#x2714; </span>
			<p>Wir testen die Werbekampagnen und sammeln laufend Daten zur Verbesserung.</p>
		</li>
		<li>
			<span> &#x2714; </span>
			<p>Wir skalieren Ihre Kampagnen so weit wie möglich oder nach Ihrer Kapazität.</p>
		</li>
		<li>
			<span> &#x2714; </span>
			<p>
				Wir stellen den Erfolg für Sie und Ihre Kampagnen sicher, solange Sie bei uns Kunde sind.
			</p>
		</li>
		<li>
			<span>&#x2714;</span>
			<p>Wir widmen uns Ihrem Geschäft, als wäre es unser eigenes.</p>
		</li>
		<li>
			<span>&#x2714;</span>
			<p>Ihr Erfolg = unser Erfolg. Das Preissystem unserer Leistungen beansprucht, dass Sie Erfolg haben müssen, damit wir profitieren.</p>
		</li>
	</ul>

	<div>
		<Incentive />
		<div class="list-image image" />
	</div>
</section>

<style>
	ul {
		list-style: none;
	}

	li {
		margin: 0.5em 0;
		display: inline-flex;
		width: fit-content;
		gap: 1em;
		align-items: center;
		padding: .5em;
		border-radius: 1em;
		background: linear-gradient(rgba(255, 255, 255, 0.075), transparent);
	}

	span {
		font-size: 0.8em;
	}

	section {
		font-size: var(--paragraph-fontsize);
		position: relative;
		transition: all 0.3s ease;
		overflow: hidden;
	}

	h2,
	ul {
		padding: 0 1rem;
		display: flex;
		flex-direction: column;
	}

	h2 {
		padding-top: 1rem;
	}

	div {
		height: 400px;
		display: flex;
		justify-content: space-between;
	}

	.list-image {
		position: relative;
		width: 100%;
		background-image: url('/assets/checklist.webp');
		background-size: 70%;
		background-position: center;
		background-repeat: no-repeat;
		filter: drop-shadow(5px 6px 3px rgba(0, 0, 0, 0.815)) hue-rotate(320deg);
	}

	@media only screen and (max-width: 840px) {
		.list-image {
			position: absolute;
			background-size: contain;
			bottom: -3em;
		}
	}
</style>
