<!-- Example4.svelte -->

<script>
    export let isRed = false;
</script>

<style>
    .thisIsRed {
        color: red;
    }
</style>

<h1 class:thisIsRed={isRed}>Hello world!</h1>