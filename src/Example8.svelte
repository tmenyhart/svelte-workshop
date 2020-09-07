<!-- Example8.svelte -->

<script>
    let count = 0;
    export { count as initialCount };

    $: someDerivedValue = `Derived value: ${count * 2}`;

    let notDerivedValue = `Not derived value: ${count}`;

    const increase = () => {
        count++;
    }

    const decrease = () => {
        count--;
    }
</script>

<button on:click={increase}>+</button>
<p>The count value is: {count}</p>
<p>{someDerivedValue}</p>
<p>{notDerivedValue}</p>
<button on:click={decrease}>-</button>