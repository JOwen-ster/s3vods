<script>
    import "$lib/styles/global.css";
	import Nav from '$lib/components/Nav.svelte';

    let { children } = $props();
</script>

<div class="layout-container">
    <Nav/>
    {@render children()}
</div>

<style>
    .layout-container {
        display: flex;
        flex-wrap: nowrap;
        flex-direction: column;
        justify-content: flex-start;
        align-items: center;
        height: 100dvh;
        width: 100%;
        margin: 0;
        padding: 0;
    }
</style>