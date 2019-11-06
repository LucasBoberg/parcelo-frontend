<script>
	import Button from '../components/Button.svelte';
	import ButtonOutline from '../components/ButtonOutline.svelte';
	import Footer from '../components/Footer.svelte';

	import { form } from 'svelte-forms';

	let email = "";

	const emailForm = form(() => ({
		email: {value: email, validators: ["required", "email"]}
	}));
</script>

<style>
	.navbar {
		position: absolute;
		top: 0;
		height: 48px;
		line-height: 48px;
		z-index: 999;
		width: 92vw;
		padding-left: 4vw;
		padding-right: 4vw;
		left: 50%;
		margin-top: 1rem;
		vertical-align: center;
		transform: translateX(-50%);
	}
	.navbar-title {
		font-size: 1.4rem;
		text-decoration: none;
	}
	.button-wrapper {
		float: right;
	}
	:global(.log-in) {
		margin-right: 1rem;
	}
	.hero {
		background-color: #E0FFEE;
		height: 80vh;
		width: 100%;
		position: relative;
		margin-bottom: 6rem;
	}
	.hero-wrapper {
		padding: 16vh 4vw 4rem 4vw;
	}
	.hero-title {
		font-size: 3.6rem;
		font-weight: 600;
		margin-bottom: 0;
	}
	.hero-subtitle {
		font-size: 1.4rem;
		margin-bottom: 2.6rem;
	}
	.hero-subtitle2 {
		font-size: 1.2rem;
		margin-top: 1rem;
	}
	.hero-form {
		position: relative;
	}
	.hero-icon-location {
		position: absolute;
		top: 50%;
		left: 1.2rem;
		transform: translateY(-50%);
	}
	.hero-input {
		background-color: #FFF;
		border: none;
		border-top-left-radius: 10px;
		border-bottom-left-radius: 10px;
		padding: 1.2rem 1.6rem 1.2rem 3rem;
		margin-right: -0.3rem;
		font-size: 0.9rem;
		outline: none;
		width: 20rem;
	}
	.hero-submit {
		background-color: #32E37F;
		border: none;
		padding: 1.2rem 1rem;
		color: #FFF;
		outline: none;
		cursor: pointer;
		font-size: 0.9rem;
		border-top-right-radius: 10px;
		border-bottom-right-radius: 10px;
		transition: background-color 0.1s ease-in-out;
	}
	.hero-submit:hover {
		cursor: not-allowed;
		background-color: rgb(48, 215, 120);
	}
	.hero-submit:disabled, .hero-submit[disabled] {
		background-color: rgb(142, 142, 142);
	}
	.hero-logo-white {
		z-index: 90;
		position: absolute;
		bottom: 0;
		right: 0;
	}
	.container {
		display: grid;
		grid-template-columns: auto auto;
		max-width: 50vw;
		margin: 10vh auto;
	}
	.wide {
		max-width: 70vw;
	}
	.grid-item {
		width: 50%;
		align-self: center;
	}
	.grid-item-40 {
		width: 40%;
	}
	.grid-item-60 {
		width: 60%;
	}
	.left {
		text-align: left;
		margin-left: 0;
		margin-right: auto;
	}
	.right {
		margin-left: auto;
		margin-right: 0;
	}
	.title {
		font-size: 2rem;
		margin-bottom: 0;
	}
	.image {
		margin: 0 auto;
		align-self: center;
		justify-self: center;
	}
	@media screen and (max-width: 1062px) {
		.hero-logo-white {
			width: 30%;
			height: auto;
		}
		.container {
			max-width: 80vw;
		}
		.con-right {
			grid-template-columns: auto 60%;
		}
		.wide-image {
			width: 22rem;
		}
  }
	@media screen and (max-width: 780px) {
		.hero-logo-black {
			width: 4rem;
		}
		.hero-title {
			font-size: 2.6rem;
		}
		.hero-subtitle {
			font-size: 1rem;
		}
		.hero-subtitle2 {
			font-size: 0.9rem;
		}

		.con-right {
			grid-template-columns: auto;
		}
		.right.wide-item {
			grid-row: 1;
		}
		.wide-item {
			text-align: center;
			width: 100%;
			margin-bottom: 1rem;
		}
		.con-app {
			grid-template-columns: auto;
		}
		.grid-item-60, .grid-item-40 {
			text-align: center;
			max-width: 90vw;
			width: 100%;
		}
	}
	@media screen and (max-width: 600px) {
		.hero-input {
			font-size: 0.8rem;
			width: 14rem;
		}
		.hero-submit {
			font-size: 0.8rem;
		}
		.image-mission {
			display: none;
		}
		.container {
			max-width: 90vw;
			grid-template-columns: auto;
		}
		.grid-item {
			width: 100%;
			max-width: 90vw;
			text-align: center;
		}
		.wireframe {
			width: 80%;
		}
	}
	@media screen and (max-width: 480px) {
		.hero-title {
			font-size: 2.2rem;
		}
		.hero-subtitle {
			font-size: 0.9rem;
		}
		.hero-subtitle2 {
			font-size: 0.8rem;
		}
		.hero-input {
			font-size: 0.8rem;
			width: 10rem;
		}
		.hero-submit {
			font-size: 0.8rem;
		}
	}
	@media screen and (max-width: 420px) {
		.hero-input {
			font-size: 0.8rem;
			width: 8rem;
		}
		.hero-submit {
			font-size: 0.8rem;
		}
		.wide-image {
			width: 80%;
		}
	}
	@media screen and (max-width: 380px) {
		.hero-title {
			font-size: 2rem;
		}
		.hero-subtitle {
			font-size: 0.9rem;
		}
		.hero-subtitle2 {
			font-size: 0.8rem;
		}
		.hero-icon-location {
			display: none;
		}
		.hero-input {
			padding-left: 1.6rem;
			font-size: 0.8rem;
			border-radius: 10px;
			width: 85%;
			margin-bottom: 1rem;
		}
		.hero-submit {
			border-radius: 10px;
			width: 100%;
			margin: 0 auto;
		}
		.wide-image {
			width: 80%;
		}
	}
	@media screen and (max-width: 320px) {
		.hero-logo-white {
			display: none;
		}
	}
</style>

<svelte:head>
	<title>Parcelo - Få det levererat, snabbt</title>
</svelte:head>

<nav class="navbar">
	<a href="/" class="navbar-title">Parcelo</a>
	<!--div-- class="button-wrapper">
		<ButtonOutline styleName="log-in" href="/log-in">Log in</ButtonOutline>
		<Button href="/sign-up">Sign up</Button>
	</!--div-->
</nav>

<div class="hero">
	<div class="hero-wrapper">
		<img class="hero-logo-black" alt="logo-black" src="bike-black-logo.svg" />
		<h2 class="hero-title">Få det levererat, snabbt</h2>
		<h4 class="hero-subtitle">och samtidigt hjälp dina lokala butiker</h4>

		<form class="hero-form" action="https://gmail.us5.list-manage.com/subscribe/post" method="POST">
			<input type="hidden" name="u" value="9e83444939d4f4f4a6beab3fd">
			<input type="hidden" name="id" value="15e3328fdf">
			<img class="hero-icon-location" alt="icon-mail" src="ic-mail.svg" />
			<input class="hero-input" autocomplete="off" type="email" name="MERGE0" id="MERGE0" placeholder="Din e-postadress" bind:value={email} class:invalid={!$emailForm.email.valid} />
			<button class="hero-submit" type="submit" disabled={!$emailForm.valid}>Få tillgång i förväg</button>
		</form>
		<h4 class="hero-subtitle2">Bli först om att få prova Parcelo.</h4>
		<!--h2 class="hero-title">Get it delivered, fast</!--h2>
		<h4 class="hero-subtitle">support you local shops</h4>
		<form-- class="hero-form">
			<img class="hero-icon-location" alt="icon-location" src="ic-location.svg" />
			<input class="hero-input" autocomplete="off" type="text" name="find" placeholder="Enter your address..." />
			<button class="hero-submit" type="submit"><img alt="submit-icon" src="arrow_right.svg"/></button>
		</form-->
	</div>
	<img class="hero-logo-white" alt="logo-white" src="bike-white-logo.svg" />
</div>

<section class="container con-left">
	<div class="grid-item left">
		<h3 class="title">Vårt Mål</h3>
		<p>Vi på Parcelo UF brinner för det lokala och satsar på att hjälpa lokala butiker och företag att nå en bredare kundkrets genom vår webbplats och app.</p>
	</div>
	<div class="grid-item">
		<img class="image image-mission" alt="mission" src="mission.svg" />
	</div>
</section>
<section class="container wide con-right">
	<div class="grid-item wide-item">
		<img class="image wide-image" alt="how" src="how.svg" />
		</div>
	<div class="grid-item right wide-item">
		<h3 class="title">Hur?</h3>
		<p>Du beställer från någon av dina lokala butiker som sedan skickar vidare din beställning till en av våra cyklister. Cyklisten levererar sedan varan hem till din dörr eller vilken annan adress som du en valt.</p>
	</div>
</section>
<section class="container con-left con-app">
	<div class="grid-item-60 left">
		<h3 class="title">Utforska appen</h3>
		<p>Appen finns snart tillgänglig på både iOS och Android.</p>
		<!--Button-- primary>Learn more</!--Button-->
	</div>
	<div class="grid-item-40">
		<img class="image wireframe" alt="app" src="app.svg" />
	</div>
</section>
<!--section class="container">
	<h3 class="title">Connected Stores</h3>
	<p>We at Parcelo UF are passionate about the local and invest wholeheartedly in helping local shops and companies to reach onebroader clientele through our website and app.</p>
</!--section>
<section-- class="container">
	<h3 class="title">Our Sponsors</h3>
	<p>We at Parcelo UF are passionate about the local and invest wholeheartedly in helping local shops and companies to reach onebroader clientele through our website and app.</p>
</section-->
<Footer />