<script lang="ts">
	export let id: string, name: string
	const [width, height]: number[] = [100, 100]
	const center: number = Math.min(width, height) / 2
</script>

<a href="#/{id}">
	<svg {width} {height}>
		<circle cx={center} cy={center} r=48 fill="var(--nord01)" />
	</svg>
	<p style="margin: 0;">{name}</p>
</a>
