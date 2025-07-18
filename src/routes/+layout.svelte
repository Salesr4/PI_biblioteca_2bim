<script lang="ts">
	import Cabecalho from '$lib/componentes/Cabecalho.svelte';
	import '../app.css';

	let { children } = $props();
</script>

<Cabecalho></Cabecalho>
{@render children()}
