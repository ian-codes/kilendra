<div class="gradient">
	<div class="sl1">
		<div class="gr1" />
		<div class="gr2" />
	</div>
	<div class="sl2">
		<div class="gr1" />
		<div class="gr2" />
	</div>
</div>

<div class="waves">
	<div class="w1" />
	<div class="w2" />
</div>

<style>
	.gradient {
		position: absolute;
		inset: 0;
		z-index: -10;
		height: 100%;
	}

	.sl1 {
		height: 50%;
	}

	.sl2 {
		height: 50%;
	}

	.gr1 {
		height: 50%;
		background: rgb(86, 32, 130);
		background: linear-gradient(0deg, rgba(86, 32, 130, 1) 0%, rgba(18, 181, 215, 1) 100%);
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		transform: scaleY(1.01);
	}

	.gr2 {
		height: 50%;
		background: rgb(86, 32, 130);
		background: linear-gradient(180deg, rgba(86, 32, 130, 1) 0%, rgba(18, 181, 215, 1) 100%);
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}

	.waves {
		z-index: -4;
		position: absolute;
		inset: 0;
		opacity: 1;
		mix-blend-mode: multiply;
	}

	.w1 {
		height: 50%;
		background-image: url('/assets/pattern.webp');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}

	.w2 {
		height: 50%;
		background-image: url('/assets/pattern2.webp');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}
</style>
