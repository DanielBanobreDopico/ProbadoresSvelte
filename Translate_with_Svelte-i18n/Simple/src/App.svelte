<script>

	import {dictionary,locale,_} from 'svelte-i18n';

	const translations = {
		es: {
			title: 'Bienvenido a mi sitio.',
			presentation: 'Este es un sitio para introducirse en la "localización" de aplicaciones.',
			reference: 'Referencias'
		},
		gl: {
			title: 'Benvido ó meu sitio.',
			presentation: 'Iste é un sitio para iniciarse na "localización" de aplicacións.',
			reference: 'Referencias'
		},
	}

	dictionary.set(translations);

	function toEs () {
		locale.set('es');
	}

	function toGl () {
		locale.set('gl');
	}

	toGl();
</script>

<main>
	<header>
		<span on:click={toGl}>gl</span>/<span on:click={toEs}>es</span>
	</header>
	<section>
		<h1>{$_('title')}</h1>
		<p>{$_('presentation')}</p>
	</section>
	<footer>
		<code>
			{$_('reference')}: <a href='https://lokalise.com/blog/svelte-i18n/#Internationalizing_and_Localizing_your_App_UI_with_Svelte_i18n'>Svelte i18n: A step-by-step guide</a>
		</code>
	</footer>
</main>

<style>
	header, footer, section {
		margin: 30px;
	}
	header {
		text-align: right;
	}
	footer {
		position: fixed;
		bottom: 0px;
	}
</style>
