<script>
	import Expertise from '../components/Expertise.svelte';
	import Introduction from '../components/Introduction.svelte';
</script>

<main>
	<Introduction />
	<Expertise />
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		position: relative;
		width: clamp(100px, 100%, 1100px);
		gap: 20vh;
	}
</style>
