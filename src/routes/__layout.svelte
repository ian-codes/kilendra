<script>
	import Background from '../components/Background.svelte';

	import Bubbles from '../components/Bubbles.svelte';
	import FadeIn from '../components/FadeIn.svelte';
	import Footer from '../components/Footer.svelte';
	import Header from '../components/Header.svelte';
</script>


<FadeIn />
<Header />
<slot />
<Footer />
<Background />

<style>
	@font-face {
		font-family: 'Sulphur';
		src: url('/fonts/Sulphur_Point/SulphurPoint-Regular.ttf') format('truetype');
	}
	@font-face {
		font-family: 'Cinzel';
		src: url('/fonts/Cinzel/Cinzel-VariableFont_wght.ttf') format('truetype');
	}
	@font-face {
		font-family: 'DM Sans';
		src: url('/fonts/DM_Sans/DMSans-Regular.ttf') format('truetype');
	}
	:global(:root) {
		--padding-default: 16px 32px;
		--margin-default: 40px 0;
		--paragraph-fontsize: 1.5rem;
		--h2-fontsize: 3rem;
		font-size: 16px;
		letter-spacing: 1px;
	}
	:global(*) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}
	:global(*::selection) {
		color: black;
		text-shadow: 0 0 1px black;
	}
	:global(h2) {
		font-size: 3rem;
		margin: 2rem 0;
	}
	:global(body) {
		position: relative;
		display: flex;
		flex-direction: column;
		align-items: center;
		overflow-x: hidden;;
		font-family: 'DM Sans';
		color: white;
		min-height: 100vh;
	}
</style>
