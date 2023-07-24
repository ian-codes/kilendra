<div />

<style>
	div {
        pointer-events: none;
		inset: 0;
		position: absolute;
		z-index: 20;
		background: black;
        animation: fadeIn 2s ease-in forwards;
	}

	@keyframes fadeIn {
		0% {
			opacity: 1;
		}
		99% {
			opacity: 0;
		}
		100% {
            opacity: 0;
			display: none;
		}
	}
</style>
