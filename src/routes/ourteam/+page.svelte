<script>
	import TeamMemper from '../../component/ourteam/TeamMemper.svelte';
</script>

<svelte:head>
	<meta name="description" content="Meet the dedicated team behind Abaqira Academy's primary and kindergarten education excellence">
    <meta name="keywords" content="Our Team, Abaqira Academy Staff, Education Professionals">
    <title>Our Team at Abaqira Academy</title>
</svelte:head>
<main>
	<h1>Our Leadership Team</h1>
	<TeamMemper
		src="Abdulaziz.png"
		nameOfmember="AbdulAziz Mahammad"
		titleOfmember="The CEO & Founder of the Academy"
		dateOfmember="Since 2013"
	/>
	<TeamMemper
		src="Neima.png"
		nameOfmember="Neima Mahammad"
		titleOfmember="Founder & Manager of the Kinder Garden"
		dateOfmember="Since 2013"
	/>
	<TeamMemper
		src="Khiru.png"
		nameOfmember="Heiru Mohammed"
		titleOfmember="Manager of the primary school"
		dateOfmember="Since 2013"
	/>
</main>

<style>
	main {
		display: grid;
		place-items: center;
	}
	main h1 {
		color: #000;
		text-align: center;
		margin: 1rem;
		font-family: var(--ff-DM-Sans);
		font-size: 19.048px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
		letter-spacing: 0.476px;
	}
	@media screen and (min-width: 800px){
		main h1{
		font-size: 4rem;

		}
	}
</style>
