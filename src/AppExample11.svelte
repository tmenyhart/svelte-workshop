<!-- AppExample11.svelte -->

<script>
    import Example10 from './Example10.svelte';

    let isLoggedIn = false;

    let onLoginButtonClick = () => {
        isLoggedIn = true;
    };

    let onLogoutButtonClick = () => {
        isLoggedIn = false;
    };
</script>

<Example10
    isLoggedIn={isLoggedIn}
    onLoginButtonClick={onLoginButtonClick}
    onLogoutButtonClick={onLogoutButtonClick}
/>