<script>
	export let heading;
	export let paragraph;
</script>

<div class="about-text">
	<h1>{heading}</h1>
	<p>{paragraph}</p>
</div>

<style>
	:root{
		--bg-color: #384cff;
		--text-color: #fff;
	}
	.about-text {
		width: var(--Main-width);
		background-color: var(--bg-color);
		margin-top: 1rem;
		padding: 2rem;
		border-radius: 20px;
	}
	.about-text h1 {
		font-family: var(--ff-DM-Sans);
		font-weight: 500;
		font-size: 27px;
		color:var(--text-color);

		line-height: normal;
	}
	.about-text p {
		color: var(--text-color);
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 15.2px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
	}
	@media screen and (min-width: 800px) {
		.about-text{
		padding: 4rem;
		border-radius: 50px;

		}
		.about-text h1 {
			font-family: var(--ff-DM-Sans);
			font-weight: 500;
			font-size: 96px;
			color: var(--text-color);

			line-height: normal;
		}
		.about-text p {
			color:var(--text-color);
			text-align: justify;
			font-family: var(--ff-Open-Sans);
			font-size: 40px;
			font-style: normal;
			font-weight: 400;
			line-height: 1.5;
		}
	}
</style>
