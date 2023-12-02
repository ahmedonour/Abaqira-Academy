<script>
	export let src;
	export let alt;
	export let nameOfmember;
	export let titleOfmember;
	export let dateOfmember;
</script>

<div class="teamMember">
	<img {src} {alt} />
	<div class="memberInfo">
		<h1>
			{nameOfmember}
		</h1>
		<p>
			{titleOfmember}
		</p>
		<p>
			{dateOfmember}
		</p>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
	}
	.teamMember {
		display: inline-flex;
		padding: 12px 30px 1px 30px;
		flex-direction: column;
		justify-content: flex-end;
		align-items: center;
		gap: 28.19px;
		margin-block: 1rem;
	}
	.teamMember img {
		border-radius: 20px;
	}
	.teamMember .memberInfo {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.teamMember .memberInfo h1 {
		font-family: var(--ff-DM-Sans);
		font-size: 1rem;
		font-weight: 700;
	}
	.teamMember .memberInfo p:nth-of-type(1) {
		font-size: 11.43px;
		font-family: var(--ff-Open-Sans);
		padding-bottom: 8px;
		border-bottom: 1px solid #000;
		font-weight: 400;
	}
	.teamMember .memberInfo p:nth-of-type(2) {
		font-size: 19px;
		font-weight: 600;
		margin-top: 10px;
		font-family: var(--ff-Open-Sans);
	}
	@media screen and (min-width: 800px) {
		.teamMember {
			flex-direction: row;
			justify-content: space-between;
			width: 80vw;
			margin-block: 3rem;
		}
		.teamMember .memberInfo h1 {
			font-family: var(--ff-DM-Sans);
			font-size: 2rem;
			font-weight: 900;
		}
		.teamMember .memberInfo p:nth-of-type(1) {
			font-size: 1rem;
			font-family: var(--ff-Open-Sans);
			padding-bottom: 8px;
			border-bottom: 1px solid #000;
			font-weight: 600;
		}
		.teamMember .memberInfo p:nth-of-type(2) {
			font-size: 19px;
			font-weight: 600;
			margin-top: 10px;
			font-family: var(--ff-Open-Sans);
		}
	}
</style>
