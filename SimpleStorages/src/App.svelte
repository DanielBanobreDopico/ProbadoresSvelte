<script>
	import Comp1 from './Comp1.svelte';
    import { name } from './store.js';
</script>

<main>
<h1>App</h1>
Nombre: {$name}
<Comp1/>
</main>