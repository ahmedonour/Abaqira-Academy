<script>
	export let ProgramTitle;
	export let src;
	export let alt;
	export let description;
</script>

<div class="program">
	<h1>{ProgramTitle}</h1>
	<div class="programDetails">
		<img {src} {alt} />
		<p>{description}</p>
	</div>
</div>

<style>
	:root {
		--ff-size: 100%;
	}
	.program {
		width: 100vw;
		padding-top: 1.5rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		/* gap: 2rem; */
	}
	.program h1 {
		color: #000;
		text-align: center;
		font-family: var(--ff-DM-Sans);
		font-size: clamp(1.2rem, 4vw, 2rem);
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	.program .programDetails {
		width: 300px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.program .programDetails img {
		width: 100%;
		height: 100%;

		margin-block: 1.2rem;
		border-radius: 25px;
	}
	.program .programDetails p {
		color: #000;
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 15.203px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
	}
	@media screen and (min-width: 800px) {
		.program {
			padding: 0rem;
			width: 80vw;
			margin-top: 1rem;
			align-items: flex-start;
		}

		.program h1 {
			margin-bottom: 1.5rem;
			color: #000;
			font-family: var(--ff-DM-Sans);
			font-size: clamp(1rem, 4vw, 4rem);
			font-style: normal;
			font-weight: 700;
			line-height: normal;
		}
		.program .programDetails img {
			margin-block: 0px;
		}
		.program .programDetails p {
			font-size: 25px;
		}
		.program .programDetails {
			gap: 2rem;
			height: 435px;
			width: 100%;
			display: flex;
			flex-direction: row;
			align-items: flex-start;
			justify-content: center;
		}
	}
</style>
