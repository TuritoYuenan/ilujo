<script lang="ts">
	export let toolName: string = ""
</script>

<svelte:head>
	<title>{toolName} | Ilujo</title>
</svelte:head>

<header>
	<h2>{toolName}</h2>
</header>

<style>
	header {text-align: center; font-variant: small-caps;}
</style>
