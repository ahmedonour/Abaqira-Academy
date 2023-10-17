<script>
	import { onMount } from 'svelte';
	import { fly } from 'svelte/transition';

	let isVisible = false;

	onMount(() => {
		// Trigger the transition after a delay or based on some condition
		setTimeout(() => {
			isVisible = true;
		}, 1000); // Delay the transition for 1 second
	});
</script>

<section class="Hero">
	<div class="hero-text">
		<h1>Abaqira Academy</h1>
		<p>Home Of Genius</p>
		<p class="hero-desktop">
			At Abaqira Academy, we ignite young minds and shape tomorrow's leaders. Nestled in the vibrant
			heart of Addis Ababa, our school is a beacon of quality education, dedicated to nurturing
			young talents while celebrating the rich cultural diversity of Ethiopia.
		</p>
	</div>
	<div class="hero-img">
		<img
			src="star.svg"
			alt=""
			srcset=""
			id="star"
			in:fly={{ x: -200, duration: 500 }}
			out:fly={{ x: 200, duration: 500 }}
		/>
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img src="Hero-image.png" alt="Image Of Studant" srcset="" />
		<img src="book.svg" alt="" srcset="" id="cube" />
	</div>
	<div class="hero-button">
		<a href="/about"><button>Read More</button></a>
	</div>
</section>

<style>
	.Hero {
		width: 80vw;
		margin-top: 26px;
		display: flex;
		justify-content: space-between;
		align-items: center;
		flex-direction: column;
	}
	.hero-text {
		display: inline-flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 6px;
	}
	.hero-text h1 {
		font-family: var(--ff-DM-Sans);
		font-weight: 700;
		font-size: 36px;
	}
	.hero-text p {
		font-family: var(--ff-Open-Sans);
		font-weight: 400;
		font-size: 30px;
	}
	.hero-text .hero-desktop {
		display: none;
	}
	.hero-img {
		margin-top: 35px;
	}
	.hero-img #star,
	#cube {
		display: none;
	}
	.hero-img img {
		border-radius: 140px;
	}
	.hero-button {
		margin-top: 40px;
	}
	.hero-button a button {
		display: flex;
		width: 44.0675vw;
		height: 50px;
		padding: 12.346px 27.864px 12.654px 27.778px;
		justify-content: center;
		align-items: center;
		flex-shrink: 0;
		font-family: var(--ff-Open-Sans);
		font-size: 18;
		font-weight: 800;
		border-radius: 12.346px;
		border: 4px solid #000;
		background: #fff;
		columns: #000;
	}
	.hero-button a button:hover {
		background-color: #000;
		color: #fff;
	}
	@media screen and (min-width: 800px) {
		.Hero {
			display: grid;
			grid-template-columns: repeat(1fr, 2);
			grid-column-gap: 1rem;
			grid-template-rows: 50px 370px 80px;
			margin-top: 20px;
			margin-bottom: 20px;
			align-items: center;
			max-width: 90vw;
			max-height: 604px;
		}
		.hero-img {
			margin-top: 0;
			max-width: 405px;
			max-height: 608px;
			grid-column: 2;
			grid-row: 1 / span 3;
		}
		.hero-img img {
			width: 100%;
			height: 100%;
			border-radius: 200px;
		}
		.hero-img #star,
		#cube {
			display: block;
			border-radius: 0;
		}
		.hero-img #star {
			position: relative;
			right: 20px;
			top: 90px;
			max-height: 190px;
			max-width: 190px;
			z-index: 2;
		}
		.hero-img #cube {
			position: relative;
			bottom: 200px;
			left: 100px;
			max-height: 200px;
			max-width: 200px;
		}
		.hero-text {
			justify-content: center;
			align-items: flex-start;
			grid-column: 1;
			grid-row: 2/3;
			grid-column-gap: 1rem;
		}
		.hero-text h1 {
			color: #000;
			font-family: var(--ff-DM-Sans);
			font-size: 80px;
			font-style: normal;
			font-weight: 700;
			line-height: normal;
			letter-spacing: 2.25px;
		}
		.hero-text p {
			color: #000;
			font-family: var(--ff-Open-Sans);
			font-size: 50px;
			font-style: normal;
			font-weight: 400;
			line-height: normal;
			letter-spacing: 1.25px;
		}
		.hero-button {
			grid-row: 3/3;
			grid-column: 1;
			gap: 60px;
		}
		.hero-text .hero-desktop {
			max-width: 620px;
			max-height: 150px;
			display: block;
			color: #000;
			text-align: justify;
			font-family: var(--ff-DM-Sans);
			font-size: 23.25px;
			font-style: normal;
			font-weight: 400;
			line-height: normal;
			letter-spacing: 0.581px;
		}
		.hero-button a button {
			width: 200px;
			height: 50px;
			display: inline-flex;
			/* padding: 20px 46px 20px 45px; */
			justify-content: center;
			align-items: center;
			border-radius: 15px;
			background: #384cff;
			color: #fff;
			font-size: 1.2rem;
			cursor: pointer;
		}
		.hero-button a button:hover {
			background: #fff;
			color: #384cff;
		}
	}
</style>
