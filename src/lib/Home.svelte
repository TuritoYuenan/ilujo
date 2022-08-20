<script lang="ts">
	import Tool from "./modules/Tool.svelte";

	const Tools = [
		{ id: "luxmeter", name: "Lux Meter" },
		{ id: "netmeter", name: "Speedtest" },
		{ id: "calculat", name: "Calculator" },
		{ id: "capturer", name: "Camera"}
	];

	const Convs = [
		{ id: "convarea", name: "Area" },
		{ id: "convmass", name: "Mass" },
		{ id: "convtime", name: "Time" },
	];
</script>

<header style="font-variant: small-caps;">
	<h1>Ilujo</h1>
</header>
<main>
	<h2>Tools</h2>
	<section class="grid">
		{#each Tools as { name, id }}<Tool {name} {id} />{/each}
	</section>
	<h2>Converters</h2>
	<section class="grid">
		{#each Convs as { name, id }}<Tool {name} {id} />{/each}
	</section>
</main>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
	}
</style>
