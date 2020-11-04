<script>
    import { name } from './store.js';
    async function addQuestion () {
        $name += '?';
    }
</script>

<h3>Componente 2</h3>
<p>Nombre: {$name}</p>
<button on:click={addQuestion}>{$name}</button>