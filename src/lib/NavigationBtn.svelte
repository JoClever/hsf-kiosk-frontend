<script>
	let { category, active = false, onclick } = $props();

	let classes = $derived(`flex size-16 rounded-lg transition duration-300 ${active ? "bg-red-900 dark:bg-stone-600" : ""}`);
</script>

<button class={classes} aria-pressed={active} {onclick}>
	<img class="" src="https://www.hsf-ev.de/files/20221102_hsf_logo-header.svg" alt={category} />
</button>
