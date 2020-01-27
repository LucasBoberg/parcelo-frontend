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
	<h1>Användarvillkor</h1>
	<h2>Allmänt</h2>
	<p>Det är inte tillåtet att använda Parcelo på vis som skulle strida mot svensklagstiftning, eller i annan kriminell verksamhet. Vid överträdelse kan polisanmälan komma att göras.</p>
	<h2>Vi registrerar personuppgifter i samband med</h2>
	<p>Ditt besök hos Parcelo, inklusive men inte endast begränsat till trafikdata, platsdata, webbloggar samt annan kommunikationsdata såsom till exempel, IP-adress, typ av enhet, operativsystem, ort eller webbläsare typ.</p>
	<h2>Ditt samtycke</h2>
	<p>Genom att du använder Parcelo godkänner du till att de personuppgifter, som ditt namn, telefonnummer och e-postadress, du fyller i på olika platser på denna webbplats får användas i markandsföringssyfte för den tjänst som exponeras i anslutning till där du ombeds fylla i dina personuppgifter. Vi samlar även in din IP-adress, geografisk position och intressen i syfte att kunna bättre anpassa vår marknadsföring till dig.</p>
	<p><i>När du klickar på knappen ”Jag samtycker” samtycker du även till att vi från Parcelo får lägga en så kallad tredjepartscookie på din dator. Denna cookie kommer att följa dig och ditt surfbeteende i syfte att kunna erbjuda dig marknadsföring som baseras på ditt beteende </i></p>
	<h2>Hur din data används</h2>
	<ul>
		<li>Analyser av marknadsundersökningar.</li>
		<li>Statistisk data om våra besökare, som beteende men alltid på aggregerad nivå.</li>
		<li>Genom analyser utvecklas och förbättras våra tjänster.</li>
		<li>Personuppgifter används även vid analys för att utföra segmentering/profilering, för att kunna utveckla riktade erbjudanden och tjänster</li>
		<li>För att kunna ge dig relevanta rekommendationer, erbjudanden och anpassade tjänster baserat på vad andra med liknande beteendemönster har intresserat sig för, vad du har valt för tjänst, tittat på och visat intresse för.</li>
		<li>För att hjälpa oss utveckla webbplatsen för att bli mer användbara och för att förbättra användarupplevelsen.</li>
		<li>För att skicka viktig information såsom meddelanden angående förändringar i våra villkor och policyer.</li>
	</ul>
	<h2>Information som kan lämnas ut</h2>
	<p>Vi kan dela med oss av data till företag som behandlar information åt oss, allt för att vi ska kunna utföra våra tjänster. Exempel skulle kunna vara analys, distribution eller andra tjänster för att upprätthålla och tillämpa våra användarvillkor. Vi hantering av data iakttas säkerhet i den mån vi klarar av att säkerställa. Parcelo samarbetar endast med partners som behandlar personuppgifter inom EU/EES eller med företag som upprätthåller samma skyddsnivå som inom EU/EES genom att t.ex. ha anslutit sig till den s.k. Privacy Shield överenskommelsen mellan EU och USA.</p>
	<h2>Rättslig grund, lagring och gallring av personuppgifter</h2>
	<p>Dina personuppgifter kommer lagras och kan brukas i marknadsföringssyfte alternativt på sätt som nämnts ovan. NOTERA, du kan närsomhelst återkalla ditt samtycke genom att kontakta oss, för kontaktuppgifter se under rubriken Kontakt.</p>
	<p>All behandling av data sker enligt Svensk Lagstiftning vilket innebär att data kommer inte sparas längre än vad som är nödvändigt. Information kommer gallras ut allt eftersom den saknar aktualitet eller annat nödvändigt syfte. Viss information kan hända att bevaras längre till följd av lagkrav.</p>
	<h2>Dina rättigheter</h2>
	<p>Du har rättigheter när det gäller dina personuppgifter och du har möjlighet att påverka din information och vad som sparas. Företaget kommer på eget eller kundens initiativ att rätta uppgifter som upptäcks vara felaktiga. Du kan även närsomhelst begära att dina uppgifter raderas eller att dess användning begränsas genom att kontakta oss (för kontakt se under rubriken Kontakt). Om du anser att dina rättigheter inte respekteras av oss får du gärna kontakta oss eller höra av dig till datainspektionen (datainspektionen@datainspektionen.se).</p>
	<h2>Länkar till utomstående webbplatser</h2>
	<p>I händelse av att vår webbplats innehåller länkar till tredje parts webbplatser, hemsidor, eller material publicerat hos tredje part, är dessa länkar endast för informationssyfte. Eftersom Företaget saknar kontroll över innehållet på dessa webbplatser eller dess material ansvarar vi därför inte för dess innehåll. Företaget ansvarar inte heller för skador eller förluster som skulle kunna uppstå vid användning av dessa länkar.</p>
	<h2>Kontakt</h2>
	<p>E-postadress: <a href="mailto:kontakt@parcelo.se">kontakt@parcelo.se</a></p>
</div>

<Footer/>