<div class="gradient" />
<div class="sky" />
<div class="curve"/>

<style>
	.gradient {
		pointer-events: none;
		z-index: -6;
		position: absolute;
		inset: 0;
		height: 100%;
		background: linear-gradient(rgb(35, 135, 165), #231446);
		box-shadow: 0 3px 5px rgba(10, 16, 34, 0.87);
	}
	.sky {
		z-index: -5;
		height: 100%;
		width: 100%;
		position: absolute;
		inset: 0;
		background-image: url('/assets/sky.jpg');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		opacity: 0.2;
		mix-blend-mode: multiply;
		box-shadow: 0 0 30px 5px black;
	}
/* 	.curve {
		z-index: -6;
		position: absolute;
		background: #231446;
		width: 100%;
		height: 10vh;
		border-radius: 0 0 100rem 100rem / 10rem;
		bottom: 0;
	} */
</style>
