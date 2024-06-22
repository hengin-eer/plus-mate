<script>
    import Icon from '@iconify/svelte';
    export let iconName;
    export let actionTitle;
    export let actionMethod;
</script>

<button on:click={() => actionMethod()}>
    <div class="leftIcon">
        <Icon icon={iconName} />
    </div>
    <p>{actionTitle}</p>
</button>

<style>
    button {
        padding: 8px 12px;
        padding-right: 16px;
        border: solid 1px black;
        border-radius: 8px;
        
        display: flex;
        align-items: center;
        gap: 4px;

        color: black;
        background-color: var(--background);
    }
    button>.leftIcon {
        width: 32px;
        height: 32px;
    }

    button>p {
        margin: 0;
        font-size: 16px;
        line-height: 1.0;
    }
</style>
