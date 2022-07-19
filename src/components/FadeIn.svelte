<div />

<style>
	div {
        pointer-events: none;
		width: 100%;
		height: 100%;
		inset: 0;
		position: absolute;
		z-index: 10;
		background: linear-gradient(rgb(35, 135, 165), rgb(35, 20, 70));
        animation: fadeIn 3s ease forwards;
	}
	@keyframes fadeIn {
		0% {
			opacity: 1;
		}
		50% {
			opacity: 0;
		}
		100% {
            opacity: 0;
			display: none;
		}
	}
</style>
