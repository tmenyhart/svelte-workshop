<!-- Example9.svelte -->

<script>
    let numbers = [1, 2, 3, 5];
    export { numbers as initialNumbers };

    $: sum = numbers.reduce((acc, curr) => acc + curr, 0);

    $: if (numbers.length === 4) {
        alert('Wow, you are really good with numbers!');
    }

    const addOne = () => {
        numbers = [...numbers, 1];
    }

    const addTwo = () => {
        numbers.push(2);
        numbers = numbers;
    }

    let untouchedValue = 1;

    $: thisWillNotReRender = `The untouched value is: ${untouchedValue}`;
</script>

<button on:click={addOne}>Add 1</button>
<button on:click={addTwo}>Add 2</button>
<p>The sum is: {sum}</p>
<p>The numbers are: {numbers}</p>
<p>{thisWillNotReRender}</p>