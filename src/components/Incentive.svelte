<div>
	<a href="#schedule">
		<p>Beratungsgespräch</p>
		<span>Unverbindlich & 100% kostenlos</span>
	</a>
</div>

<style>
	div {
		z-index: 10;
		height: 10rem;
		display: flex;
		align-items: center;
		justify-content: left;
		margin-top: 1rem;
		margin-left: 1rem;
		transition: all 0.2s ease;
	}

	div:hover {
		transform: scale(1.07);
	}
	div:hover a {
		background: linear-gradient(-90deg, rgb(16, 151, 185), rgb(18, 80, 150));
	}

	span {
		font-size: 0.5em;
		font-weight: normal;
	}

	a {
		text-decoration: none;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 0.2em;
		cursor: pointer;
		width: 12em;
		font-size: 1em;
		font-weight: bold;
		border-radius: 5px;
		padding: 0.8em;
		background: linear-gradient(90deg, rgb(118, 40, 182), rgb(15, 38, 143));
		box-shadow: 0px 8px 10px rgba(0, 0, 0, 0.5), 0 -1px 2px rgba(255, 255, 255, 0.841);
		color: white;
		border: none;
		transition: all 0.2s ease;
	}

	a:focus {
		outline: 3px dotted white;
	}


	@media only screen and (max-width: 840px) {
		div {
			margin-top: 0;
			margin-right: 0;
			justify-content: center;
		}
		a {
			width: 11em;
		}
	}

	@media only screen and (max-width: 325px) {
		a {
			width: 9em;
		}

		span {
			font-size: 0.4em;
		}
	}
</style>
