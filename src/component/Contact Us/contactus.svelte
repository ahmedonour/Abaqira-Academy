<script>
</script>

<main>
	<div class="contact-title">
		<div class="line" />
		<h1>Contact Us</h1>
		<p>Let's Get In Touch</p>
		<p>
			We're excited to hear from you and be a part of your child's educational journey at Abaqira
			Academy. Whether you have questions, suggestions, or simply want to say hello, we're here and
			ready to assist you.
		</p>
		<div class="deg90">
			<p>Warm regards, The Abaqira Academy Team</p>
		</div>
	</div>
	<form action="https://formsubmit.co/info@abaqiraacademy.com" method="POST">
		<input type="text" name="name" id="name" placeholder="Name" />
		<input type="email" name="email" id="email" placeholder="Email" />
		<textarea name="Message" id="message" cols="30" rows="5" placeholder="Message" />
		<button type="submit">Send</button>
	</form>
</main>

<style>
	:root {
		--fs-heading: 3.3rem;
		--fs-ContactUs: 1.35rem;
		--padding-inline: 25px;
	}
	main {
		width: 80vw;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: auto;
		padding: 45px var(--padding-inline);
		background-color: #384cff;
		border-radius: 20px;
	}
	main .contact-title {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		grid-template-rows: 30px 130px;
	}
	main .contact-title .line {
		background-color: #fff;
		align-self: center;
		height: 1px;
		width: 100px;
		grid-row: 1;
		grid-column: 1;
	}
	main .contact-title h1 {
		grid-row: 1;
		grid-column: 2;
		align-self: flex-start;
		color: #fff;
		text-align: justify;
		font-family: var(--ff-DM-Sans);
		font-size: var(--fs-ContactUs);
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	main .contact-title p:nth-of-type(1) {
		color: #fff;
		font-family: var(--ff-DM-Sans);
		font-size: var(--fs-heading);
		font-style: normal;
		font-weight: 700;
		line-height: normal;
		grid-row: 2;
		grid-column: 1 / span 2;
	}
	form {
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		width: 100%;
		height: auto;
		flex-wrap: wrap;
		gap: 1rem;
		margin-top: 1rem;
	}
	form input {
		background-color: transparent;
		width: 100%;
		border: none;
		border-bottom: 2px solid #fff;
		outline: none;
		font-size: 1rem;
		padding: 0.5rem;
		color: #fff;
		font-family: var(--ff-Open-Sans);
	}
	form input::placeholder {
		position: fixed;
		color: #fff;
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 17.241px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	form textarea {
		background-color: transparent;
		width: 100%;
		border: none;
		font-size: 1rem;
		outline: none;
		font-family: var(--ff-Open-Sans);
		color: #fff;

		border-bottom: 2px solid #fff;
	}
	form textarea::placeholder {
		color: #fff;
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 17.241px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	form button {
		display: flex;
		width: 100%;
		padding: 10.345px 0px 9.759px 0px;
		justify-content: center;
		align-items: center;
		border-radius: 8.621px;
		background: #fff;
		border: none;
		color: #000;
		text-align: justify;
		font-family: var(--ff-Open-Sans);
		font-size: 17.241px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
		cursor: pointer;
		border: 1px solid #fff;

		transition: all 1s ease-in-out;
	}
	main .contact-title p:nth-of-type(2) {
		display: none;
	}
	main .contact-title .deg90 p {
		display: none;
	}
	form button:hover {
		background-color: #384cff;
		color: #fff;
	}
	@media screen and (max-width: 320px) {
		:root {
			--fs-heading: 2.8rem;
			--fs-ContactUs: 1rem;
		}
	}
	@media screen and (min-width: 800px) {
		:root {
			--fs-heading: 6rem;
			--fs-ContactUs: 2.5rem;
			--fs-p: 20px;
			--padding-inline: 40px;
		}
		main {
			width: 71vw;
			flex-direction: row;
			height: 70vh;
		}
		main .contact-title {
			width: 50%;
			height: auto;
			display: grid;
			grid-template-columns: 200px 230px 30px;
			grid-template-rows: repeat(auto-fill, min(30px));
			gap: 1rem;
		}
		main .contact-title .line {
			background-color: #fff;
			align-self: center;
			height: 2px;
			width: 200px;
			grid-row: 1;
			grid-column: 1;
		}
		main .contact-title h1 {
			grid-row: 1;
			grid-column: 2;
			align-self: flex-start;
			color: #fff;
			text-align: justify;
			font-family: var(--ff-DM-Sans);
			font-size: var(--fs-ContactUs);
			font-style: normal;
			font-weight: 700;
			line-height: normal;
		}
		main .contact-title p:nth-of-type(1) {
			font-size: var(--fs-heading);
			grid-column: 1 / span 3;
		}
		main .contact-title p:nth-of-type(2) {
			display: block;
			color: #fff;
			text-align: justify;
			font-family: var(--ff-Open-Sans);
			font-size: var(--fs-p);
			font-style: normal;
			font-weight: 400;
			line-height: normal;
			grid-row: 3;
			grid-column: 1 / span 2;
		}
		main .contact-title .deg90 {
			place-self: center;
			width: 490px;
			height: 30px;
			transform: rotate(-90deg);
			grid-row: 1 / span 3;
			grid-column: 3;
		}
		main .contact-title .deg90 p {
			display: block;
			color: #fff;
			text-align: center;
			font-family: var(--ff-Open-Sans);
			font-size: 1.2rem;
			font-style: oblique;
			font-weight: 800;
			line-height: normal;
		}
		form {
			width: 50%;
			display: flex;
			justify-content: flex-end;
			align-items: center;
			margin-top: 0;
			height: 100%;
		}
		form input {
			width: 50%;
		}
		form textarea {
			width: 50%;
		}
		form button {
			width: 50%;
		}
	}
	@media screen and (max-height: 700px) {
		:root {
			--fs-heading: 6rem;
			--fs-ContactUs: 2rem;
			--fs-p: 15px;
		}
	}
</style>
