<script>
	let isOpen = false

	function handleBurgerClick() {
		isOpen = !isOpen
	}
</script>

<header id="home">
	<a class="logo" href="/">
		Kilendra
	</a>

	<nav>
		<button on:click={handleBurgerClick} id="burger">
			<span></span>
			<span></span>
			<span></span>
		</button>
		<ol class="{isOpen ? "open" : "closed"}">
			<li>
				<a class="menuLink" href="#home">
					Home
				</a>
			</li>
			<li>
				<a class="menuLink" href="#how-we-work">
					Wie wir arbeiten
				</a>
			</li>
			<li>
				<a class="menuLink" href="#get-in-touch">
					Kontakt
				</a>
			</li>
		</ol>
	</nav>
</header>

<style>
	header {
		font-family: 'DM Sans', Arial;
		margin-top: 4rem;
		margin-bottom: 8rem;
		display: flex;
		justify-content: space-between;
		align-items: center;
		width: 100%;
		max-width: 1100px;
		padding: 0 1rem;
		position: relative;
	}

	.logo {
		font-size: 3em;
	}
	
	nav {
		height: 100%;
	}
	
	#burger {
		display: none;
	}
	ol {
		display: flex;
		align-items: center;
		justify-content: space-between;
		list-style: none;
		gap: 5em;
	}
	li a {
		color: white;
		text-decoration: none;
		font-size: 1.2em;
		font-weight: bold;
	}
	a {
		position: relative;
		transition: all 0.2s ease;
	}
	li a::after {
		content: '';
		position: absolute;
		background: white;
		bottom: -5px;
		left: 0;
		height: 2px;
		width: 0;
		transition: all .2s ease;
	}
	.menuLink:hover {
		text-shadow: 0 0 10px rgba(0, 0, 0, 0.233);
	}
	a:hover::after {
		width: 100%;
	}

	@media only screen and (max-width: 840px) {
		header {
			margin: 2rem 1rem;
			margin-bottom: 3em;
			width: 100%;
			flex-direction: column;
			align-items: start;
		}
		#burger {
			position: absolute;
			top: 1.5em;
			right: 1rem;
			background: none;
			border: none;
			width: 30px;
			height: 30px;
			display: flex;
			flex-direction: column;
			justify-content: space-between;
			cursor: pointer;
		}
		#burger span {
			height: 3px;
			width: 100%;
			background: white;
		}
		a {
			font-size: 2em;
			border-right: none;
			margin-bottom: .5rem;
		}
		nav {
			width: 100%;
		}
		ol {
			width: 100%;
			display: none;
			flex-direction: column;
			gap: 1em;
			align-items: end;
		}
		li {
			padding: .5em 1em;
			/* background: linear-gradient(transparent, rgba(255, 255, 255, 0.082)); */
		}
		li a {
			font-weight: lighter;
		}
		.open {
			display: flex !important;
		}
	}
</style>
