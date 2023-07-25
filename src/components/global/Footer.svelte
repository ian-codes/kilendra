<footer>
	<div class="logoContainer">
		<a class="logo" href="/">Kilendra</a>
	</div>

	<div class="copyright">
		<p>Copyright &#169; 2023 Kilendra. All Rights Reserved.</p>
		<p>Made with &#9829; in Switzerland.</p>
	</div>
</footer>

<style>
	footer {
		font-family: 'DM Sans';
		margin: 3rem;
		display: flex;
		flex-direction: column;
		align-items: center;
		gap: 1em;
	}

	.copyright {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: start;
		opacity: .7;
		gap: .5em;
	}

	@media only screen and (max-width: 840px) {
		footer {
			padding: 2rem 2rem;
			width: 100%;
			align-items: center;
			margin-bottom: 2em;
		}
		.copyright {
			font-size: 0.8rem;
		}
		.copyright > p {
			text-align: center;
		}
	}
</style>
