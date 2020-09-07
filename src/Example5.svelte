<!-- Example5.svelte -->

<script>
    export let padding = '4px';
</script>

<style>
    h1 {
        background-color: red;
        padding: var(--padding);
    }
</style>

<h1 style='--padding:{padding}'>Hello world!</h1>