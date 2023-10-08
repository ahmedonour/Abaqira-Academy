<script>
	import AboutText from '../../component/About Page /About-text.svelte';
</script>

<main>
	<div class="about-title">
		<h1>About Us</h1>
	</div>
	<AboutText
		heading="Who We Are"
		paragraph="Welcome to Abaqira Academy, an educational institution dedicated to excellence in Addis Ababa, Ethiopia. Founded with a vision to provide a holistic and culturally enriching learning experience, Abaqira Academy has been a beacon of quality education for the community since its inception."
	/>
	<AboutText
		heading="Our Story"
		paragraph="Abaqira Academy was established in 2013 with a passion for nurturing young minds and fostering a sense of belonging within our diverse community. We recognized the need for an educational institution that not only excels academically but also embraces and celebrates Ethiopia's rich cultural heritage. Our journey began with a commitment to provide an exceptional learning environment where students can thrive academically, morally, and socially."
	/>
	<AboutText
		heading="Our Mission"
		paragraph="At Abaqira Academy, our mission is to empower students with knowledge, character, and a deep appreciation for their Ethiopian heritage. We strive to:"
	/>
	<ol>
		<li>Foster Academic Excellence:</li>
		<p>
			We offer a curriculum that meets and exceeds national standards, ensuring that our students
			are well-prepared for their academic journey.
		</p>
		<li>Cultivate Cultural Awareness:</li>
		<p>
			We celebrate Ethiopia's diverse culture and heritage, promoting inclusivity and respect for
			all backgrounds.
		</p>
		<li>Nurture Moral Values:</li>
		<p>
			We instill in our students a strong sense of ethics, responsibility, and compassion, shaping
			them into responsible citizens.
		</p>
		<li>Promote Holistic Development:</li>
		<p>
			Beyond academics, we focus on developing well-rounded individuals, encouraging creativity,
			critical thinking, and leadership skills.
		</p>
		<li>Inspire Lifelong Learning:</li>
		<p>
			We cultivate a love for learning that goes beyond the classroom, equipping students with the
			tools they need to thrive in an ever-changing world.
		</p>
	</ol>
	<AboutText
		heading="Our Approach"
		paragraph="Abaqira Academy takes a holistic approach to education, recognizing that each child is unique and has their own strengths and talents. We provide a supportive and nurturing environment where students can explore their interests, develop their skills, and build their character. Our dedicated faculty members are passionate about education and work tirelessly to ensure that every student reaches their full potential."
	/>
	<AboutText
		heading="Join the Abaqira Family"
		paragraph="We invite you to become a part of the Abaqira family, where every student is valued, every culture is celebrated, and every mind is empowered. Whether you are a parent seeking the best education for your child or a student eager to embark on a journey of discovery, we welcome you to explore our website, visit our campus, and experience firsthand the warmth and excellence that define Abaqira Academy."
	/>
	<p>
		Thank you for considering us as your partner in your educational journey. Together, we can shape
		a brighter future for our children and our nation.
	</p>
	<p id="last">“Empowering Minds, Enriching Lives.”</p>
</main>

<style>
	main {
		display: grid;
		place-items: center;
	}
	main .about-title {
		display: inline-flex;
		padding: 6px 84.904px 6.69px 84px;
		justify-content: center;
		align-items: center;
	}
	main h1 {
		color: #000;
		font-family: var(--ff-DM-Sans);
		font-size: 20px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
		letter-spacing: 0.5px;
	}
	main ol {
		font-family: var(--ff-Open-Sans);
		max-width: 75vw;
	}
	main ol li {
		color: #000;
		font-family: Open Sans;
		font-size: 15.2px;
		font-style: normal;
		font-weight: 700;
		line-height: normal;
	}
	main ol p {
		color: #000;
		text-align: justify;
		font-family: Open Sans;
		font-size: 15.2px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
	}
	main p {
		width: var(--Main-width);
		color: #000;
		text-align: justify;
		font-family: Open Sans;
		font-size: 15.2px;
		font-style: normal;
		font-weight: 400;
		line-height: normal;
	}
	main #last {
		margin-top: 1rem;
		color: #000;
		font-family: Open Sans;
		font-size: 15.2px;
		font-style: italic;
		font-weight: 700;
		line-height: normal;
	}
</style>
