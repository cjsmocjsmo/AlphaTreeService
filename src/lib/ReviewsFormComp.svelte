<script>
	import { db } from '$lib/firebase';
	import { setDoc, doc } from 'firebase/firestore';

	let currentDate = new Date();
	let cDay = currentDate.getDate();
	let cMonth = currentDate.getMonth() + 1;
	let cYear = currentDate.getFullYear();

	let name = '';
	let email = '';
	let message = '';
	let date = cDay + '-' + cMonth + '-' + cYear;
	let formIsActive = true;
	
	const approved = 'no';
	const quarintine = 'yes';
	const del = 'no';

	let time = currentDate.getHours() + currentDate.getMinutes() + currentDate.getSeconds();
	let uuid = date + time
	let title = 'review' + uuid;

	async function setReview() {
		console.log(message);
		await setDoc(doc(db, 'reviews', title), {
			UUID: uuid,
			Date: date,
			Name: name,
			Email: email,
			Sig: email,
			Message: message,
			Approved: approved,
			Quarintine: quarintine,
			Delete: del
		});
	}

	function handleClick() {
		setReview();
		formIsActive = false;
	}

	
</script>

<h3>Post A Review:</h3>
{#if formIsActive}
	<input
		bind:value={name}
		placeholder="Name (optional)"
		id="name"
		class="foo"
		type="text"
		name="name"
	/>
	<br />
	<input bind:value={email} placeholder="Email" id="email" class="foo" type="text" name="email" />
	<br />
	<textarea bind:value={message} id="message" name="message" rows="8" cols="30" />
	<br />
	<button on:click={handleClick} id="revInput" class="foo">Post Review</button>
{:else}
	<p class="postrev">Thank you for your review. </p>
{/if}

<style>
	.postrev {
		color: antiquewhite;
		font-size: 1.5em;
	}

	h3 {
		color: antiquewhite;
		font-size: 3em;
	}

	textarea {
		background-color: rgb(6, 40, 134);
		font-size: 1.83em;
		color: antiquewhite;
		width: 80%;
	}

	.foo {
		font-size: 2em;
		background-color: bisque;
	}

	@media (max-width: 412px) {
		textarea {
			font-size: 1.57em;
		}
		.foo {
			font-size: 1.71em;
		}
	}

	@media (max-width: 378px) {
		textarea {
			font-size: 1.43em;
		}
		.foo {
			font-size: 1.6em;
		}
	}
</style>
