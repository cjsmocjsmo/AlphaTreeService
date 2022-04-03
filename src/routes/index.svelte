<script>
	import BannerComp from '$lib/Banner.svelte';
	import MainImageComp from '$lib/MainImageComp.svelte';
	import MissionComp from '$lib/MissionComp.svelte';
	import MainDivComp from '$lib/MainDivComp.svelte';
	import ReviewsComp from '$lib/ReviewsComp.svelte';
	import ReviewsFormComp from '$lib/ReviewsFormComp.svelte';
	import FooterComp from '$lib/FooterComp.svelte';
	import NavButton from '$lib/images/NavButton.svelte';
</script>

<body>
	<BannerComp />
	<div class="revform">
		<MainImageComp />
		<MissionComp />

		<iframe
			class="foo-vid"
			width="335"
			height="595"
			src="https://www.youtube.com/embed/adLBtc5uBwM"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
			allowfullscreen
		/>

		<iframe
			class="maind-vid"
			width="700"
			height="400"
			src="https://www.youtube.com/embed/M4ZGLJk7Cjw"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
			allowfullscreen
		/>

		<MainDivComp />

		<iframe
			class="maind-vid"
			width="700"
			height="400"
			src="https://www.youtube.com/embed/PHDLlOBqkjw"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
			allowfullscreen
		/>

		<ReviewsComp />
		<ReviewsFormComp />
		<NavButton />
	</div>
	<FooterComp />
</body>

<style>
	body {
		background-color: black;
	}

	.revform {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-evenly;
	}

	.maind-vid {
		margin-top: 6em;
		margin-bottom: 4em;
		border-radius: 12px;
	}

	.foo-vid {
		border-radius: 12px;
	}

	@media (max-width: 812px) {
		.maind-vid {
			margin-top: 6em;
			margin-bottom: 4em;
		}
	}

	@media (max-width: 712px) {
		.maind-vid {
			margin-top: 6em;
			margin-bottom: 4em;
		}
	}

	@media (max-width: 612px) {
		.maind-vid {
			width: 100%;
			margin-top: 3em;
			margin-bottom: 2em;
		}
	}

	@media (max-width: 512px) {
		.maind-vid {
			width: 100%;
			margin-top: 3em;
			margin-bottom: 2em;
		}
	}

	@media (max-width: 415px) {
		.maind-vid {
			width: auto;
			height: auto;
			margin-top: 3em;
			margin-bottom: 2em;
		}
	}
</style>
