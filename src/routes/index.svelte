<script>
	import Button from '../components/Button.svelte';
	import ButtonOutline from '../components/ButtonOutline.svelte';
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
	}
	.hero-submit:hover {
		background-color: rgb(48, 215, 120);
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
		text-align: right;
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
</style>

<svelte:head>
	<title>Parcelo</title>
</svelte:head>

<nav class="navbar">
	<a href="/" class="navbar-title">Parcelo</a>
	<div class="button-wrapper">
		<ButtonOutline styleName="log-in" href="/log-in">Log in</ButtonOutline>
		<Button href="/sign-up">Sign up</Button>
	</div>
</nav>

<div class="hero">
	<div class="hero-wrapper">
		<img class="hero-logo-black" alt="logo-black" src="bike-black-logo.svg" />
		<h2 class="hero-title">Get it delivered, fast</h2>
		<h4 class="hero-subtitle">support you local shops</h4>
		<form class="hero-form">
			<img class="hero-icon-location" alt="icon-location" src="ic-location.svg" />
			<input class="hero-input" autocomplete="off" type="text" name="find" placeholder="Enter your address..." />
			<button class="hero-submit" type="submit"><img alt="submit-icon" src="arrow_right.svg"/></button>
		</form>
	</div>
	<img class="hero-logo-white" alt="logo-white" src="bike-white-logo.svg" />
</div>

<section class="container">
	<div class="grid-item left">
		<h3 class="title">Our Mission</h3>
		<p>We at Parcelo UF are passionate about the local and invest wholeheartedly in helping local shops and companies to reach onebroader clientele through our website and app.</p>
	</div>
	<div class="grid-item">
		<img class="image" alt="mission" src="mission.svg" />
	</div>
</section>
<section class="container wide">
	<div class="grid-item">
		<img class="image" alt="how" src="how.svg" />
		</div>
	<div class="grid-item right">
		<h3 class="title">How?</h3>
		<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip</p>
	</div>
</section>
<section class="container">
	<div class="grid-item-60 left">
		<h3 class="title">Explore the app</h3>
		<p>Check out the app available on iOS and Android.</p>
		<Button primary>Learn more</Button>
	</div>
	<div class="grid-item-40">
		<img class="image" alt="app" src="app.svg" />
	</div>
</section>
<section class="container">
	<h3 class="title">Connected Stores</h3>
	<p>We at Parcelo UF are passionate about the local and invest wholeheartedly in helping local shops and companies to reach onebroader clientele through our website and app.</p>
</section>
<section class="container">
	<h3 class="title">Our Sponsors</h3>
	<p>We at Parcelo UF are passionate about the local and invest wholeheartedly in helping local shops and companies to reach onebroader clientele through our website and app.</p>
</section>