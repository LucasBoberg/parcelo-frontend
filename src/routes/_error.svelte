<script>
	import Button from '../components/Button.svelte';
	import Footer from '../components/Footer.svelte';
	export let status;
	export let error;

	const dev = process.env.NODE_ENV === 'development';
</script>

<style>
	div.wrapper {
		position: relative;
		background-color: #E0FFEE;
		text-align: center;
		width: 100vw;
		height: calc(100vh - 280px);
		display: flex;
		align-items: center;
		justify-content: center;
	}

	h1, p {
		width: 100%;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	p {
		margin: 1em auto;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>

<svelte:head>
	<title>{status}</title>
</svelte:head>

<div class="wrapper">

	<div>
		<h1>{status}</h1>

		<p>{error.message}</p>

		{#if dev && error.stack}
			<pre>{error.stack}</pre>
		{/if}
		<Button href="/">Tillbaka till sidan</Button>
	</div>
</div>

<Footer/>