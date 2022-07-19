<script>
	import Incentive from './Incentive.svelte';
	import LogoRoster from './LogoRoster.svelte';

	function handleHover() {
		return 1;
	}
</script>

<section>
	<h2>Our Area of Expertise</h2>
	<LogoRoster />
	<p>
		We at Kilimandred mainly do one thing - <b>paid advertisement</b>. This is what we are fully
		committed to and what we do best. Our tried and tested ad strategies are robust and offer
		tremendous returns for clients that we've worked with.
	</p>
	<br />
	<p>
		We run ads on the largest media platforms; Facebook, Google, TikTok and Instagram. Depending
		on the client and our ad strategy, we will choose a certain platform over another.
	</p>
	<Incentive />
</section>

<style>
	section {
		position: relative;
		margin: 1rem;
	}
	h2 {
		font-size: var(--h2-fontsize);
	}
	p {
		font-size: var(--paragraph-fontsize);
		margin-left: 0;
	}
</style>
