<script>

	import {locale} from 'svelte-i18n';

    function toEs () {
		locale.set('es');
	}

	function toGl () {
		locale.set('gl');
	}

</script>

<header>
    <span on:click={toGl}>gl</span>/<span on:click={toEs}>es</span>
</header>

<style>
    header {
        margin: 30px;
        text-align: right;
    }
</style>
