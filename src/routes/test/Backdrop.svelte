<script lang="ts">
	import { fade } from 'svelte/transition'
</script>

<div
	aria-hidden="true"
	style="background-color: green; height: 20px;"
	transition:fade|global={{ duration: 2000 }}
>
	2
</div>
