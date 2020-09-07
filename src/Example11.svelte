<!-- Example11.svelte -->

<script>
    let items = [
        { id: 'id0', name: 'Item 1'},
        { id: 'id1', name: 'Item 2'},
        { id: 'id2', name: 'Item 3'},
        { id: 'id3', name: 'Item 4'},
    ];

    const onRemoveLastClick = () => {
        if (items.length) {
            items.pop();
            items = items;
        }
    };

</script>

<ul>
{#each items as item, index}
   <li>Index: {index}, Id: {item.id}, Name: {item.name}</li>
{/each}
</ul>
<button on:click={onRemoveLastClick}>Remove last item</button>
