<script>
	import Router from "svelte-spa-router";

	import Home from "./lib/Home.svelte";
	import ConvArea from "./lib/tools/ConvArea.svelte";
	import ConvMass from "./lib/tools/ConvMass.svelte";
	import ConvTime from "./lib/tools/ConvTime.svelte";
	import MeterLux from "./lib/tools/MeterLux.svelte";
	import MeterNet from "./lib/tools/MeterNet.svelte";
	import Calcultr from "./lib/tools/Calcultr.svelte";
	import Capturer from "./lib/tools/Capturer.svelte";
</script>

<Router
	routes={{
		"/": Home,
		"/convarea/": ConvArea, // Area Converter
		"/convmass/": ConvMass, // Mass Converter
		"/convtime/": ConvTime, // Time Converter
		"/luxmeter/": MeterLux, // Lux Meter
		"/netmeter/": MeterNet, // Internet Speedtest
		"/calculat/": Calcultr, // Calculator
		"/capturer/": Capturer, // Camera
	}}
/>
