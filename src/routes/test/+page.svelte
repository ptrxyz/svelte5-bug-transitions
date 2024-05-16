<script lang="ts">
	import Backdrop from './Backdrop.svelte'

	import { fade } from 'svelte/transition'

	let showTheThing = $state(false)
</script>

<button onclick={() => (showTheThing = !showTheThing)}>Toggle</button>

{#if showTheThing}
	<div
		aria-hidden="true"
		style="background-color: red; height: 20px;"
		transition:fade|global={{ duration: 2000 }}
	>
		1
	</div>
	<Backdrop></Backdrop>
{/if}
