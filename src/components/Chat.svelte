<div>
	<div class="chat" />
</div>

<style>
	div {
		z-index: -4;
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 27em;
		opacity: 0.8;
		filter: drop-shadow(2px 4px 20px rgba(0, 0, 0, 0.308));
	}
	.chat {
		background: linear-gradient(90deg, rgb(81, 185, 211), rgba(149, 115, 168, 0.479));
		clip-path: polygon(0% 0%, 100% 0%, 100% 40%, 74% 40%, 81% 51%, 46% 38%, 0 38%);
	}
	@keyframes pulse {
		0% {
			filter: hue-rotate(0);
		}
		50% {
			filter: hue-rotate(120deg);
		}
		100% {
			filter: hue-rotate(0);
		}
	}
</style>
