<script>
	import cloudflare from '$lib/images/cloudflare.svg';
	import firebase from '$lib/images/firebase.svg';
</script>

<section class="section2">
	<p class="footerNum">360 516 8933</p>
	<div class="bar">
		<div class="addr1">
			<p class="footerp">251 East Snow Cap Dr</p>
			<p class="footerp">Belfair, WA 98528</p>
			<p class="footerp">United States</p>
		</div>
		<br />
		<div class="addr1">
			<p class="footerp">License</p>
			<p class="footerp">WA #604-037-042</p>
		</div>
		<br />
		<div class="addr1">
			<p class="footerp">Insurance</p>
			<p class="footerp">#SII4851A201464</p>
			<p class="footerp">Contractors Insurance NW</p>
			<p class="footerp">PO Box 13033</p>
			<p class="footerp">Olympia WA 98508</p>
		</div>
		<br />
		<div class="addr1">
			<p class="footerp">Bond</p>
			<p class="footerp">#62922843</p>
			<p class="footerp">Department Of Labor and Industries</p>
			<p class="footerp">Contractor Registration</p>
			<p class="footerp">PO Box 44450</p>
			<p class="footerp">Olympia WA 98504-4450</p>
		</div>
	</div>
	<div class="logo-div">
		<img class="fb" src={firebase} alt="fuckit"/>
		<img class="cf" src={cloudflare} alt="fuckit"/>
	</div>
</section>

<style>

	.fb {
		width: 35%;
	}

	.cf {
		width: 50%;
	}


	section.section2 {
		background-color: blue;
		margin-top: 3em;
	}

	.footerNum {
		text-align: center;
		font-size: 5em;
		color: antiquewhite;
	}

	.bar {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}

	.addr1 {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 10px;
	}

	.logo-div {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		margin-top: 3em;
	}

	p.footerp {
		font-weight: 700;
		font-size: 3.5em;
		color: antiquewhite;
	}

	@media (max-width: 2010px) {
		p.footerp {
			font-size: 2em;
		}
	}

	@media (max-width: 1810px) {
		p.footerp {
			font-size: 1.75em;
		}
	}

	@media (max-width: 1710px) {
		p.footerp {
			font-size: 1.55em;
		}
	}

	@media (max-width: 1310px) {
		p.footerp {
			font-size: 1.25em;
		}
	}

	@media (max-width: 1010px) {
		p.footerp {
			font-size: 1em;
		}
		.footerNum {
			font-size: 4.25em;
		}
	}

	@media (max-width: 845px) {
		.bar {
			flex-direction: column;
		}
		p.footerp {
			font-size: 1.5em;
		}

		.logo-div {
			flex-direction: column;
		}
	}

	@media (max-width: 540px) {
		p.footerp {
			font-size: 1.75em;
		}
	}

	@media (max-width: 412px) {
		p.footerp {
			font-size: 1.1em;
		}

		.footerNum {
			font-size: 2.7em;
		}
	}

	@media (max-width: 331px) {
		p.footerp {
			font-size: 1.1em;
		}

		.footerNum {
			font-size: 2.7em;
		}
	}
</style>
