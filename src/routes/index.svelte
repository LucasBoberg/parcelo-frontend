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
		vertical-align: center;
		transform: translateX(-50%);
	}
	.navbar-title {
		font-size: 1.4rem;
		line-height: 48px;
		margin: 0;
	}
	.hero {
		background-color: #F4FDF8;
		height: 80vh;
		position: relative;
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
		border-top-left-radius: 5px;
		border-bottom-left-radius: 5px;
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
		border-top-right-radius: 5px;
		border-bottom-right-radius: 5px;
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
</style>

<svelte:head>
	<title>Parcelo</title>
</svelte:head>

<nav class="navbar">
	<h1 class="navbar-title">Parcelo</h1>
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
