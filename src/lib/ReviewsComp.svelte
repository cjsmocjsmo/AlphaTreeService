<script>
	import { db } from '$lib/firebase';
	import { collection, query, where, getDocs } from 'firebase/firestore';

	async function getReviews() {
		let zoo = [];
		const q = query(
			collection(db, 'reviews'),
			where('Approved', '==', 'yes'),
			where('Quarintine', '==', 'no'),
			where('Delete', '==', 'no')
		);
		const querySnapshot = await getDocs(q);
		let qhs = querySnapshot.forEach((rev) => {
			let ace = rev.data();
			zoo.push(ace);
		});
		return zoo;
	}
	let reviews = getReviews();
</script>

<div class="review1">
	{#await reviews}
		<p>...waiting</p>
	{:then message}
		{#each message as M}
			<div class="rev-card">
				<div class="rev-card-body">
					<h2 class="rev-card-title">Review</h2>
					<p class="rev-cbod">{M.Message}</p>
					<p class="rev-csig">{M.Sig}</p>
				</div>
			</div>
		{/each}
	{/await}
</div>

<style>
	.rev-card-title {
		color: antiquewhite;
		text-align: center;
		font-size: 3em;
	}

	.rev-csig {
		color: antiquewhite;
		text-align: right;
		padding-right: 15px;
	}

	.rev-cbod {
		color: antiquewhite;
		padding: 10px;
		font-size: 1.5em;
	}

	.review1 {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-items: top;
		justify-content: space-evenly;
		background-color: rgb(6, 40, 134);

		border: 4px solid yellowgreen;
		border-radius: 7px;
		margin: 1em;
		width: 100%;
	}

	@media (max-width: 331px) {
		.review1 {
			flex-direction: column;
			align-items: center;
			justify-content: center;
		}
	}
</style>
