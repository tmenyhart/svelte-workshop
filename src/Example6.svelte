<!-- Example6.svelte -->

<script>
    function onButtonClick() {
        alert('Hello world!');
    }
</script>

<button on:click={onButtonClick}>Press me!</button>