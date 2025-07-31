<script lang="ts">
    import { onMount } from "svelte"

    let text = $state("...")
    onMount(async () => {
        let res = await fetch("/api")
        text = await res.text()
    })
</script>

<h1>Welcome to SvelteKit</h1>
<p>{text}</p>
