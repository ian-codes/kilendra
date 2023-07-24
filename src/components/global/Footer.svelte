<footer>
	<a class="logo" href="/">Kilendra</a>


	<div class="copyright">
		<p>Copyright &#169; 2022 Kilimandred.</p>
		<p>All Rights Reserved.</p>
		<br />
		<p>Made with &#9829; in Switzerland.</p>
	</div>
</footer>

<style>
	footer {
		font-family: 'DM Sans';
		margin: 3rem;
	}
	.logo {
		font-size: 3em;
		font-weight: bold;
		text-decoration: none;
		color: white;
	}
	.copyright {
		display: flex;
		align-items: center;
		flex-direction: column;
		opacity: .7;
	}
	a {
		transition: all 0.2s ease;
	}
	a:hover {
		text-shadow: 0 0 20px rgba(0, 0, 0, 0.377);
	}

	@media only screen and (max-width: 840px) {
		footer {
			padding: 2rem 2rem;
			width: 100%;
			flex-direction: column;
			margin-bottom: 2em;
		}
		.logo {
			flex-direction: column;
			align-items: center;
			justify-content: space-between;
		}
		.copyright {
			align-items: center;
			justify-content: center;
			font-size: 0.8rem;
		}
		.copyright > p {
			text-align: center;
		}
		a {
			font-size: 2em;
			border-right: none;
			border-bottom: 1px dotted rgba(255, 255, 255, 0.87);
			margin-bottom: 0.5rem;
			padding: 0.1em 0.4em;
		}
		span {
			font-size: 0.8rem;
			margin: 0;
		}
	}
</style>
