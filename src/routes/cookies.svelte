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
	.text-wrapper {
		padding: 12vh 4vw;
		width: 40vw;
		margin: 0 auto;
	}
	bold {
		font-weight: 700;
	}
	@media screen and (max-width: 1024px) {
		.text-wrapper {
			width: 60vw;
		}
	}
	@media screen and (max-width: 640px) {
		.text-wrapper {
			width: 80vw;
		}
	}
</style>

<svelte:head>
	<title>Parcelo - Thank You!</title>
</svelte:head>

<nav class="navbar">
	<a href="/" class="navbar-title">Parcelo</a>
</nav>

<div class="text-wrapper">
	<h1>Cookies</h1>
	<p>
		Hos Parcelo använder vi oss av så kallade cookies I enlighet med lagen om elektronisk kommunikation ska alla som besöker webbplatsen få information om: 
	</p>
	<ul>
		<li>att cookies används</li>
		<li>hur de används</li>
		<li>hur cookies undviks</li>
	</ul>
	<h2>Cookies används när allmännyttig information delges</h2>
	<p>Vi behöver i enstaka fall meddela alla våra besökare något och för att informationen inte ska behöva dyka upp flera gånger används cookies.</p>
	<h2>Cookies för statistik</h2>
	<p>För att vi på Parcelo ska kunna ge dig den bästa upplevelsen och det är därmed av stor vikt att kunna få korrekt och oberoende besöksstatistik. Statistiken används för att ge den bästa möjliga upplevelse för våra användare. NOTERA, Statistiken är alltid på aggregerad nivå.</p>
	<h2>Så stänger du av cookies</h2>
	<p>Vill du inte att dina cookies ska sparas kan du stänga av dem i din webbläsares inställningar, då kommer inga cookies att sparas. NOTERA, stängs cookies av kan delar av webbplatsen få begränsad brukbarhet samt delar kan även bli obrukbara.</p>
	<h2>Vad är en cookie?</h2>
	<p>En cookie är en textfil som webbplatsen sparar på din dator för att ge besökaren funktioner. Informationen i en cookie möjliggör möjligheten att följa användares surfande. Det finns två typer av cookies:</p>
	<p><bold>Den första</bold> är en fil som sparas en längre tid på din dator. Den används vid funktioner som exempel talar om vad som är nytt sedan användaren senast besökte hemsidan.</p>
	<p><bold>Den andra</bold> typen så kallade sessionscookies är en temporär cookie som endast är aktiv under tiden du är inne och surfar på webbplatsen. Sessionscookies sparas inte under längre tid på din dator utan försvinner när webbläsaren stängs.</p>
</div>

<Footer/>