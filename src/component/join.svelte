<script>
	export let Heading;
	export let Desc;
</script>

<main>
	<h1>{Heading}</h1>
	<p>{Desc}</p>
	<p><i>Empowering Minds, Enriching Lives.</i></p>
	<button>Join Us Now</button>
</main>

<style>
	main {
		font-family: var(--ff-Open-Sans);
		margin-top: 1rem;
		padding: 1rem;
		line-height: 1.5;
		width: 80vw;
		display: flex;
		flex-direction: column;
	}
	main p {
		font-size: 1rem;
		text-align: justify;
	}
	main p:nth-of-type(2) {
		font-weight: 900;
	}
	main button {
        display: none;
        position: relative;
		cursor: pointer;
		transition: all 1s ease-in-out;
		/* align-self: end; */
		border-radius: 20px;
		margin-block: 1rem;
		background: var(--Contact-bg, #384cff);
		border: none;
		color: #fff;
		padding: 1rem 2rem;
		border-radius: 15px;
		font-weight: 800;
		font-size: 1rem;
		font-family: var(--ff-Open-Sans);
	}
	main button:hover {
		background-color: #9fa7f5;
		color: #000;
	}
	@media screen and (min-width: 800px) {
		main {
			padding: 0;
		}
		main p {
			font-size: 30px;
		}
		main button {
        bottom: 50px;

			margin-block: 0;
			align-self: end;
		}
	}
</style>
