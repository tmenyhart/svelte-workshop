<!-- Example10.svelte -->

<script>
    export let isLoggedIn;
    
    export let onLoginButtonClick = () => {};
    export let onLogoutButtonClick = () => {};
</script>

{#if isLoggedIn}
    <button on:click={onLogoutButtonClick}>Logout</button>
{:else}
    <button on:click={onLoginButtonClick}>Login</button>
{/if}

{#if isLoggedIn}
    <p>You are logged in</p>
{/if}

{#if !isLoggedIn}
    <p>You are logged out</p>
{/if}
