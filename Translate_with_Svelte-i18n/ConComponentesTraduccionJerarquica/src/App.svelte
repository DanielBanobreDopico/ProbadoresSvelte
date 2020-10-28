<script>

	import {dictionary,locale} from 'svelte-i18n';

	import {translations} from './translations.js';

	import Header from './Header.svelte';
	import Contents from './Contents.svelte';
	import Footer from './Footer.svelte';

	dictionary.set(translations);

	locale.set('gl');

</script>

<main>
	<Header/>
	<Contents/>
	<Footer/>
</main>

<style>
</style>