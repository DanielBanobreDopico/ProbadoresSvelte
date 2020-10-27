<script>

	import {dictionary,locale} from 'svelte-i18n';

	import {translations} from './translations.js';

	import Encabezado from './Encabezado.svelte';
	import Contidos from './Contidos.svelte';
	import Pie from './Pie.svelte';

	dictionary.set(translations);

	locale.set('gl');

</script>

<main>
	<Encabezado/>
	<Contidos/>
	<Pie/>
</main>

<style>
</style>