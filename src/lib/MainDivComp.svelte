<script>
	import kitsap from '$lib/images/kitsap.webp';
	import mason from '$lib/images/mason.webp';
	import pierce from '$lib/images/pierce.webp';
</script>

<div class="mainDiv">
	<section class="sec">
		<p class="teleNum">360 516 8933</p>
		<p class="atsServ">Servicing</p>
		<div class="cardDiv">
			<div class="card">
				<div class="card-body">
					<h1 class="card-title">Kitsap County</h1>

					<div>
						<img class="cardImg" src={kitsap} alt="Placeholder" />
					</div>
				</div>
			</div>
			<div class="card">
				<div class="card-body">
					<h1 class="card-title">Mason County</h1>
					<div>
						<img class="cardImg" src={mason} alt="Placeholder" />
					</div>
				</div>
			</div>
			<div class="card">
				<div class="card-body">
					<h1 class="card-title">Pierce County</h1>
					<div>
						<img class="cardImg" src={pierce} alt="Placeholder" />
					</div>
				</div>
			</div>
		</div>
		<div class="gallery">
			<a href="https://alphatreeservicegallery.pages.dev">
				<p class="p-gallery">Photo Gallery</p>
			</a>
			<a href="https://alphatreeservicevids.pages.dev">
				<p class="p-gallery">Video Gallery</p>
			</a>
		</div>
		<br />
	</section>
</div>

<style>
	.mainDiv {
		margin-top: 1.5em;
		width: 100%;
	}

	.sec {
		background-color: rgb(6, 40, 134);
		border: 4px solid yellowgreen;
		border-radius: 10px;
	}

	.teleNum {
		margin-top: 0.5em;
		text-align: center;
		font-size: 5em;
		font-weight: 900;
		color: antiquewhite;
	}

	.atsServ {
		text-align: center;
		font-size: 4.5em;
		color: antiquewhite;
	}

	.cardDiv {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-evenly;
	}

	.card-title {
		color: antiquewhite;
		text-align: center;
	}

	.cardImg {
		border-radius: 8px;
		width: 100%;
	}

	div.gallery {
		margin-top: 1.5em;
		margin-bottom: 2.5em;
	}

	p.p-gallery {
		color: antiquewhite;
		text-align: center;
		font-size: 3em;
	}

	@media (max-width: 512px) {
		.cardDiv {
			flex-direction: column;
			height: fit-content;
		}
	}

	@media (max-width: 375px) {
		.teleNum {
			margin-top: 0.5em;
			text-align: center;
			font-size: 2em;
			font-weight: 900;
			color: antiquewhite;
		}
		.atsServ {
			text-align: center;
			font-size: 1.85em;
			color: antiquewhite;
		}
		.cardDiv {
			flex-direction: column;
		}
		.cardImg {
			width: 200px;
		}
	}
</style>
