<script>
</script>

<main>
	<div class="contact-title">
		<div class="line" />
		<h1>Contact Us</h1>
		<p>Let's Get In Touch</p>
	</div>
	<form action="https://formsubmit.co/ahmedonour.49@gmail.com" method="POST">
		<input type="text" name="name" id="name" placeholder="Name" />
		<input type="email" name="email" id="email" placeholder="Email" />
		<textarea name="Message" id="message" cols="30" rows="10" placeholder="Message" />
		<button type="submit">Send</button>
	</form>
</main>

<style>
	main {
		width: 80vw;
		height: auto;
		padding: 45px 25px;
		background-color: #384cff;
		border-radius: 20px;
	}
    main .contact-title{
        display: grid;
        grid-template-columns: repeat(2 ,1fr);
        grid-template-rows:  30px 130px;
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
		font-size: 1.5rem;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	main .contact-title p {
		color: #fff;
		font-family: var(--ff-DM-Sans);
		font-size: 4rem;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
        grid-row: 2;
        grid-column: 1 / span2;
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
        padding: .5rem;
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
	}
</style>
