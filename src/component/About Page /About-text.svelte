<script>
	export let heading;
	export let paragraph;
</script>

<div class="about-text">
	<h1>{heading}</h1>
	<p>{paragraph}</p>
</div>

<style>
	.about-text {
		width: var(--Main-width);
	}
	.about-text h1 {
		font-family: var(--ff-DM-Sans);
		font-weight: 500;
		font-size: 27px;
		color: #000;

		line-height: normal;
	}
	.about-text p {
		color: #000;
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 15.2px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
	}
	@media screen and (min-width: 800px) {
		.about-text h1 {
			font-family: var(--ff-DM-Sans);
			font-weight: 500;
			font-size: 96px;
			color: #000;

			line-height: normal;
		}
		.about-text p {
			color: #000;
			text-align: justify;
			font-family: var(--ff-Open-Sans);
			font-size: 40px;
			font-style: normal;
			font-weight: 400;
			line-height: 1.5;
		}
	}
</style>
