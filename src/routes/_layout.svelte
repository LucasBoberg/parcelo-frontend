<script>
	import GdprBanner from '@beyonk/gdpr-cookie-consent-banner'
	import '@beyonk/gdpr-cookie-consent-banner/dist/style.css'
	import GoogleAnalytics from '../components/GoogleAnalytics.svelte';
</script>

<style>
	* {
		font-family: 'Asap', -apple-system, BlinkMacSystemFont, Segoe UI, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
	}
</style>

<GoogleAnalytics />
<main>
	<GdprBanner cookieName="cookieAccept" settingsLabel="" acceptLabel="Stäng" heading="" description="Genom att använda Parcelos tjänster godkänner du att vi <a target='_blank' rel='noopener' href='/cookies'>använder cookies</a>. Vi och våra partners verkar globalt och använder cookies,  bland annat för analys och personanpassning." on:analytics="" />
	<slot></slot>
</main>