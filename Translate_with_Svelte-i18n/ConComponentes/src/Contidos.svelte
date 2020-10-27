<script>
    import {_} from 'svelte-i18n';
</script>

<section>
    <h1>{$_('title')}</h1>
    <p>{$_('presentation')}</p>
</section>

<style>
    section {
        margin: 30px;
    }
</style>