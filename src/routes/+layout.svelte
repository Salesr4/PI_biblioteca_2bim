<script lang="ts">
	import Cabecalho from '$lib/componentes/Cabecalho.svelte';
	import '../app.css';
	import Rodape from "$lib/componentes/Rodape.svelte";

	let { children } = $props();
</script>

<Cabecalho></Cabecalho>
{@render children()}
<Rodape/>
