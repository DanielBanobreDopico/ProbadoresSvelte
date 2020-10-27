<script>
	// https://lokalise.com/blog/svelte-i18n/#Internationalizing_and_Localizing_your_App_UI_with_Svelte_i18n
	import Cabecera from './Cabecera.svelte';
	import Principal from './Principal.svelte';
	import {dictionary,locale} from 'svelte-i18n';

	import translations from './translations.js';

	dictionary.set(translations);
	locale.set('fr');
</script>

<main>
	<Cabecera/>
	<Principal/>
</main>

<style>
</style>