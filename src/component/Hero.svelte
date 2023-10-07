<script>
	import { fly } from 'svelte/transition';
</script>

<section class="Hero">
	<div class="hero-text">
		<h1>Abaqira Academy</h1>
		<p>Home Of Genius</p>
	</div>
	<div class="hero-img">
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img
			in:fly={{ delay: 250, duration: 800, x: 100 }}
			src="Hero-image.png"
			alt="Image Of Studant"
		/>
	</div>
	<div class="hero-button">
		<a href="/about"><button>Read More</button></a>
	</div>
</section>

<style>
	.Hero {
		width: 313px;
		margin-top: 26px;
		display: flex;
		justify-content: center;
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
	.hero-img {
		margin-top: 35px;
	}
	.hero-img img {
		border-radius: 140px;
	}
	.hero-button {
		margin-top: 40px;
	}
	.hero-button a button {
		display: flex;
		width: 158.643px;
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
    .hero-button a button:hover{
        background-color: #000;
        color: #fff;
    }
</style>
