<script>
    import AppExample1 from './AppExample1.svelte';
    import AppExample2 from './AppExample2.svelte';
    import AppExample3 from './AppExample3.svelte';
    import AppExample4 from './AppExample4.svelte';
    import AppExample5 from './AppExample5.svelte';
    import AppExample6 from './AppExample6.svelte';
    import AppExample7 from './AppExample7.svelte';
    import AppExample8 from './AppExample8.svelte';
    import AppExample9 from './AppExample9.svelte';
    import AppExample10 from './AppExample10.svelte';
    import AppExample11 from './AppExample11.svelte';
    import AppExample12 from './AppExample12.svelte';

    let currentExample = 1;
</script>

{#if currentExample === 1}
    <AppExample1 />
{/if}

{#if currentExample === 2}
    <AppExample2 />
{/if}

{#if currentExample === 3}
    <AppExample3 />
{/if}

{#if currentExample === 4}
    <AppExample4 />
{/if}

{#if currentExample === 5}
    <AppExample5 />
{/if}

{#if currentExample === 6}
    <AppExample6 />
{/if}

{#if currentExample === 7}
    <AppExample7 />
{/if}

{#if currentExample === 8}
    <AppExample8 />
{/if}

{#if currentExample === 9}
    <AppExample9 />
{/if}

{#if currentExample === 10}
    <AppExample10 />
{/if}

{#if currentExample === 11}
    <AppExample11 />
{/if}

{#if currentExample === 12}
    <AppExample12 />
{/if}

{#if currentExample < 0 || currentExample > 12}
    <p>Unknown example!</p>
{/if}