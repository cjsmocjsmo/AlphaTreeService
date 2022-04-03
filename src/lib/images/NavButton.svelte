<div class="fab-wrapper">
	<input id="fabCheckbox" type="checkbox" class="fab-checkbox" />
	<label class="fab" for="fabCheckbox">
		<span class="fab-dots fab-dots-1" />
		<span class="fab-dots fab-dots-2" />
		<span class="fab-dots fab-dots-3" />
	</label>
	<div class="fab-wheel">
		<a
			class="fab-action fab-action-1"
			href="https://www.facebook.com/pg/alphatreeservicecdm/services/"
		>
			<i>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="32"
					height="32"
					fill="currentColor"
					class="bi bi-facebook"
					viewBox="0 0 16 16"
				>
					<path
						d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"
					/>
				</svg>
			</i>
		</a>
		<a class="fab-action fab-action-2" href="tel:360 516 8933">
			<i>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="32"
					height="32"
					fill="currentColor"
					class="bi bi-telephone-fill"
					viewBox="0 0 16 16"
				>
					<path
						fill-rule="evenodd"
						d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z"
					/>
				</svg>
			</i>
		</a>
		<a class="fab-action fab-action-3" href="sms://+1360 516 8933">
			<i>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="32"
					height="32"
					fill="currentColor"
					class="bi bi-chat-dots-fill"
					viewBox="0 0 16 16"
				>
					<path
						d="M16 8c0 3.866-3.582 7-8 7a9.06 9.06 0 0 1-2.347-.306c-.584.296-1.925.864-4.181 1.234-.2.032-.352-.176-.273-.362.354-.836.674-1.95.77-2.966C.744 11.37 0 9.76 0 8c0-3.866 3.582-7 8-7s8 3.134 8 7zM5 8a1 1 0 1 0-2 0 1 1 0 0 0 2 0zm4 0a1 1 0 1 0-2 0 1 1 0 0 0 2 0zm3 1a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"
					/>
				</svg>
			</i>
		</a>
		<a class="fab-action fab-action-4" href="https://atsvids.pages.dev">
			<i>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="32"
					height="32"
					fill="currentColor"
					class="bi bi-youtube"
					viewBox="0 0 16 16"
				>
					<path
						d="M8.051 1.999h.089c.822.003 4.987.033 6.11.335a2.01 2.01 0 0 1 1.415 1.42c.101.38.172.883.22 1.402l.01.104.022.26.008.104c.065.914.073 1.77.074 1.957v.075c-.001.194-.01 1.108-.082 2.06l-.008.105-.009.104c-.05.572-.124 1.14-.235 1.558a2.007 2.007 0 0 1-1.415 1.42c-1.16.312-5.569.334-6.18.335h-.142c-.309 0-1.587-.006-2.927-.052l-.17-.006-.087-.004-.171-.007-.171-.007c-1.11-.049-2.167-.128-2.654-.26a2.007 2.007 0 0 1-1.415-1.419c-.111-.417-.185-.986-.235-1.558L.09 9.82l-.008-.104A31.4 31.4 0 0 1 0 7.68v-.123c.002-.215.01-.958.064-1.778l.007-.103.003-.052.008-.104.022-.26.01-.104c.048-.519.119-1.023.22-1.402a2.007 2.007 0 0 1 1.415-1.42c.487-.13 1.544-.21 2.654-.26l.17-.007.172-.006.086-.003.171-.007A99.788 99.788 0 0 1 7.858 2h.193zM6.4 5.209v4.818l4.157-2.408L6.4 5.209z"
					/>
				</svg>
			</i>
		</a>
	</div>
</div>

<style>
	* {
		box-sizing: border-box;
	}

	.fab-wrapper {
		position: fixed;
		bottom: 3rem;
		right: 3rem;
	}

	.fab-checkbox {
		display: none;
	}

	.fab {
		position: absolute;
		bottom: -1rem;
		right: -1rem;
		width: 4rem;
		height: 4rem;
		background: blue;
		border-radius: 50%;
		background: #126ee2;
		box-shadow: 0px 5px 20px #81a4f1;
		transition: all 0.3s ease;
		z-index: 1;
		border-bottom-right-radius: 6px;
		border: 1px solid #0c50a7;
	}

	.fab:before {
		content: '';
		position: absolute;
		width: 100%;
		height: 100%;
		left: 0;
		top: 0;
		border-radius: 50%;
		background-color: rgba(255, 255, 255, 0.1);
	}

	.fab-checkbox:checked ~ .fab:before {
		width: 90%;
		height: 90%;
		left: 5%;
		top: 5%;
		background-color: rgba(255, 255, 255, 0.2);
	}

	.fab:hover {
		background: #2c87e8;
		box-shadow: 0px 5px 20px 5px #81a4f1;
	}

	.fab-dots {
		position: absolute;
		height: 8px;
		width: 8px;
		background-color: antiquewhite;
		border-radius: 50%;
		top: 50%;
		transform: translateX(0%) translateY(-50%) rotate(0deg);
		opacity: 1;
		animation: blink 3s ease infinite;
		transition: all 0.3s ease;
	}

	.fab-dots-1 {
		left: 15px;
		animation-delay: 0s;
	}

	.fab-dots-2 {
		left: 50%;
		transform: translateX(-50%) translateY(-50%);
		animation-delay: 0.4s;
	}

	.fab-dots-3 {
		right: 15px;
		animation-delay: 0.8s;
	}

	.fab-checkbox:checked ~ .fab .fab-dots {
		height: 6px;
	}

	.fab .fab-dots-2 {
		transform: translateX(-50%) translateY(-50%) rotate(0deg);
	}

	.fab-checkbox:checked ~ .fab .fab-dots-1 {
		width: 32px;
		border-radius: 10px;
		left: 50%;
		transform: translateX(-50%) translateY(-50%) rotate(45deg);
	}

	.fab-checkbox:checked ~ .fab .fab-dots-3 {
		width: 32px;
		border-radius: 10px;
		right: 50%;
		transform: translateX(50%) translateY(-50%) rotate(-45deg);
	}

	@keyframes blink {
		50% {
			opacity: 0.25;
		}
	}

	.fab-checkbox:checked ~ .fab .fab-dots {
		animation: none;
	}

	.fab-wheel {
		position: absolute;
		bottom: 0;
		right: 0;
		width: 10rem;
		height: 10rem;
		transition: all 0.3s ease;
		transform-origin: bottom right;
		transform: scale(0);
	}

	.fab-checkbox:checked ~ .fab-wheel {
		transform: scale(1);
	}

	.fab-action {
		position: absolute;
		background: #0f1941;
		width: 3rem;
		height: 3rem;
		border-radius: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
		color: antiquewhite;
		box-shadow: 0 0.1rem 1rem rgba(24, 66, 154, 0.82);
		transition: all 1s ease;

		opacity: 0;
	}

	.fab-checkbox:checked ~ .fab-wheel .fab-action {
		opacity: 1;
	}

	.fab-action:hover {
		background-color: #f16100;
	}

	.fab-wheel .fab-action-1 {
		right: -1rem;
		top: 0;
	}

	.fab-wheel .fab-action-2 {
		right: 3.4rem;
		top: 0.5rem;
	}

	.fab-wheel .fab-action-3 {
		left: 0.5rem;
		bottom: 3.4rem;
	}

	.fab-wheel .fab-action-4 {
		left: 0;
		bottom: -1rem;
	}
</style>
