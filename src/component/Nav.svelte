<script>
	let isOpen = false;

	function toggleMenu() {
		isOpen = !isOpen;
	}
</script>

<nav>
	<div class="logo">
		<img src="favicon.png" alt="Abaqira Logo" />
		<div class="logo-text">
			<p>Abaqira</p>
			<p>Academy</p>
		</div>
	</div>
	<button on:click={toggleMenu}><img src="menu.svg" alt="" /></button>
	{#if isOpen}
		<ul id="mobile-nav">
			<button on:click={toggleMenu} id="close"><img src="x.svg" alt="" /></button>
			<li><a href="/" on:click={toggleMenu}>Home</a></li>
			<li><a href="/about" on:click={toggleMenu}>About</a></li>
			<li><a href="/ourteam" on:click={toggleMenu}>Our Team</a></li>
			<li><a href="ourprogram" on:click={toggleMenu}>Our Program</a></li>
			<li><a href="/contactus" on:click={toggleMenu}>Contact Us</a></li>
		</ul>
	{/if}
	<ul id="desktop-nav">
		<li><a href="/">Home</a></li>

		<li><a href="/about">About</a></li>
		<li><a href="/ourteam">Our Team</a></li>
		<li><a href="/ourprogram">Program</a></li>
		<li><a href="/contactus">Contact Us</a></li>
	</ul>
</nav>

<style>
	img {
		width: 50px;
		height: 50px;
	}
	button {
		background-color: transparent;
		cursor: pointer;
		border: none;
	}
	nav {
		margin-top: 15px;
		display: flex;
		width: var(--Main-width);
		height: 50px;
		justify-content: center;
		align-items: flex-start;
		gap: 200px;
		flex-shrink: 0;
	}
	nav #mobile-nav {
		position: absolute;
		right: 10vw;
		top: 100px;
		border: 2px solid #000;
		width: 200px;
		height: 300px;
		flex-shrink: 0;
		border-radius: 30px;
		background: rgba(255, 255, 255, 0.5);
		backdrop-filter: blur(25px);
		padding-inline-start: 25px;
		padding-top: 60px;
	}
	nav #mobile-nav li {
		font-family: var(--ff-Open-Sans);
		font-size: 22.29px;
		font-style: normal;
		font-weight: 800;
		line-height: normal;
		list-style: none;
	}
	.logo .logo-text {
		display: none;
	}
	nav #mobile-nav #close {
		position: absolute;
		top: 18px;
		right: 20px;
	}
	#desktop-nav {
		display: none;
	}
	@media screen and (min-width: 800px) {
		* {
			padding: 0;
			margin: 0;
		}
		button {
			display: none;
		}
		nav {
			height: 100px;
			width: 100vw;
			display: flex;
			justify-content: space-around;
			align-items: center;
		}
		nav .logo {
			display: flex;
			width: 185px;
			height: 70px;
			gap: 20px;
			justify-content: space-between;
		}
		nav .logo img {
			width: 70px;
			height: 70px;
		}
		nav .logo .logo-text {
			display: flex;
			flex-direction: column;
			height: 100%;
			justify-content: center;
			align-items: flex-start;
		}
		nav .logo .logo-text p {
			color: #000;
			font-family: var(--ff-DM-Sans);
			font-size: 20px;
			font-style: normal;
			font-weight: 900;
			line-height: normal;
			letter-spacing: 0.5px;
		}

		#desktop-nav {
			display: flex;
			justify-content: space-between;
			align-items: center;
			gap: 40px;
			list-style: none;
			color: #000;
			font-family: var(--ff-Open-Sans);
			font-size: 24px;
			font-style: normal;
			font-weight: 700;
			line-height: normal;
			letter-spacing: 0.6px;
		}
	}
</style>
