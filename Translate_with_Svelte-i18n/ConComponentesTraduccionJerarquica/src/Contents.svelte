<script>
    import {_} from 'svelte-i18n';
</script>

<section>
    <h1>{$_('contents.title')}</h1>
    <p>{$_('contents.presentation')}</p>
</section>

<style>
    section {
        margin: 30px;
    }
</style>