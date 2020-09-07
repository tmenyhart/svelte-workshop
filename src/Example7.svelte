<!-- Example7.svelte -->

<script>
    export let onButtonClick = () => {};
</script>

<button on:click={onButtonClick}>Press me!</button>