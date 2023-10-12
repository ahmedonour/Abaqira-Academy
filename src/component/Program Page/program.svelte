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
	.program {
		width: 100vw;
		padding: 1.875rem;
		display: grid;
		place-items: center;
	}
	.program h1 {
		color: #000;
		font-family: var(--ff-DM-Sans);
		font-size: 1.118375rem;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	.program .programDetails {
		width: 300px;
	}
	.program .programDetails img {
		width: 100%;
		margin-block: 2rem;
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
</style>
