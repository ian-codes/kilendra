<script>
	import Chat from './Chat.svelte';
	import Ghost from './Ghost.svelte';
	import Incentive from './Incentive.svelte';
</script>

<section class="description">
	<p>
		We make your business success dreams come to fruition. With our top of the line paid ad services
		we generate tangible results for you with a
		<span title="Return on Investment">ROI</span> that's hard to beat.
	</p>
	<p>Let's grow your business together.</p>
	<Ghost />
	<Chat />
	<Incentive />
</section>

<style>
	.description {
		font-size: var(--paragraph-fontsize);
		position: relative;
		padding: 2rem;
		transition: all 0.3s ease;
	}
	.description span:hover {
		text-decoration: underline;
	}
</style>
