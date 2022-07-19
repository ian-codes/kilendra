<script>
	let facebook;
	let google;
	let tiktok;
	let instagram;
</script>

<div>
	<span title="Facebook Ads" class="facebook" bind:this={facebook}/>
	<span title="Google Ads" class="google" bind:this={google}/>
	<span title="TikTok Ads" class="tiktok" bind:this={tiktok}/>
	<span title="Instagram Ads" class="instagram" bind:this={instagram}/>
</div>

<style>
	div {
		position: absolute;
		top: 0;
		right: 0;
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: center;
        gap: 2em;
		margin: 2rem 0;
	}
	.facebook {
		background-image: url('/assets/ad-logos/facebook.png');
	}
	.google {
		background-image: url('/assets/ad-logos/google.png');
	}
	.tiktok {
		background-image: url('/assets/ad-logos/tiktok.svg');
	}
	.instagram {
		background-image: url('/assets/ad-logos/instagram.png');
	}
	span {
		width: 2em;
		aspect-ratio: 1;
		background-position: center;
		background-size: cover;
		filter: saturate(0) invert(.2) drop-shadow(1px 1px 3px rgba(0, 0, 0, 0.322));
		transition: all 0.2s ease;
		mix-blend-mode: multiply;
	}
	span:hover {
		transform: scale(1.5);
        filter: saturate(1);
		animation: rainbow 6s infinite;
		mix-blend-mode:screen;
	}
	@keyframes rainbow {
		0% {
			filter: hue-rotate(0) drop-shadow(1px 1px 3px black);
		}
		100% {
			filter: hue-rotate(360deg) drop-shadow(1px 1px 3px black);
		}
	}
</style>
