<!-- AppExample8.svelte -->

<script>
    import Example7 from './Example7.svelte';

    const onButtonClick = () => {
        alert('Hello Supercharge!');
    };
</script>

<Example7 onButtonClick={onButtonClick}/>