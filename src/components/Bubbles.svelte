<script>
	import { onMount } from 'svelte';
	let bubbleWrapper;
	onMount(() => {
		for (let i = 0; i <= 10; i++) {
			const bubble = document.createElement('div');
			bubble.borderRadius = '100%';
			bubble.width = '100px';
			bubble.height = '100px';
			bubble.backgroundColor = 'red';
			bubbleWrapper.appendChild(bubble);
		}
	});
</script>

<div class="wrapper" />
<div bind:this={bubbleWrapper} class="bubbleWrapper"/>

<style>
	.bubbleWrapper {
		width: 100%;
		height: 100%;
	}
	.wrapper {
		position: absolute;
		top: 0;
		left: 0;
		z-index: -2;
		background-image: url('/assets/sky.jpg');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		height: 100%;
		width: 100%;
		opacity: 0.2;
		mix-blend-mode: multiply;
		clip-path: polygon(0 100%, 100% 100%, 100% 39%, 73% 49%, 68% 67%, 47% 49%, 0 42%);
	}
</style>
