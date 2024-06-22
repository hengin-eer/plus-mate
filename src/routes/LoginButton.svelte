<script>
	import IconButton from "./IconButton.svelte";
    const alertWithLogin = () => alert("Yes! Login!");
</script>

<IconButton
    iconName="material-symbols-light:login-outline-rounded"
    actionTitle="ログインする"
    actionMethod={alertWithLogin}
    --background="#41F494"
/>
