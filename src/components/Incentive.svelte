<div>
	<button>
		Get started today
		<span>Schedule a free consultation</span>
	</button>
</div>

<style>
	div {
		height: 9em;
		padding: 1em;
		display: flex;
		align-items: center;
		justify-content: left;
	}
	span {
		font-size: .5em;
		font-weight: normal;
	}
	button {
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: .4em;
		cursor: pointer;
		width: 12em;
		font-size: 1.2em;
		font-weight: bold;
		border-radius: 40px;
		margin: 1em;
		padding: 1.2em;
		background: linear-gradient(90deg, rgb(95, 40, 158), rgb(18, 60, 150));
		box-shadow: 0 3px 3px rgba(0, 0, 0, 0.288);
		color: white;
		border: none;
		animation: hover 3s infinite linear;
		transition: all 0.2s ease;
	}
	button:hover {
		font-size: 1.3em;
		animation: rainbow 3s infinite linear, hover 3s infinite linear;
	}
	button:focus {
		outline: 3px dotted white;
	}
	@keyframes rainbow {
		0% {
			filter: hue-rotate(0deg);
		}
		100% {
			filter: hue-rotate(360deg);
		}
	}
	@keyframes hover {
		0% {
			transform: translateY(0);
		}
		50% {
			transform: translateY(-5px);
		}
		100% {
			transform: translateY(0);
		}
	}
</style>
