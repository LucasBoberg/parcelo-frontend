<script>
	import Button from '../components/Button.svelte';
	import Footer from '../components/Footer.svelte';
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
	:global(.log-in) {
		margin-right: 1rem;
	}
	.wrapper {
		text-align: center;
		position: relative;
		height: calc(100vh - 280px);
		background-color: #E0FFEE;
	}
	.text-wrapper {
		padding: 4vw;
		width: 92vw;
		position: absolute;
		top: 50%;
		transform: translateY(-50%);
	}
</style>

<svelte:head>
	<title>Parcelo - Thank You!</title>
</svelte:head>

<nav class="navbar">
	<a href="/" class="navbar-title">Parcelo</a>
</nav>

<div class="wrapper">
	<div class="text-wrapper">
		<h1>Tack för ditt visat intresse!</h1>
		<h3 style="margin-bottom: 1rem;">Du kommer få information om när du kommer få möjlighet att testa Parcelo på din email.</h3>
		<Button href="/">Tillbaka till sidan</Button>
	</div>
</div>

<Footer/>