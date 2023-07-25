<script>
	import Background from '../components/Background.svelte';
	import FadeIn from '../components/FadeIn.svelte';
	import Footer from '../components/global/Footer.svelte';
	import Header from '../components/global/Header.svelte';
	import '../app.css';
</script>

<div>
	<Header />
	<slot />
	<Footer />
	<Background />
</div>

<style>
	div {
		margin: 1rem;
	}
</style>