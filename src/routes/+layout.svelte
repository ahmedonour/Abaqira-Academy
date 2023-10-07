<script>
	import Nav from "../component/Nav.svelte";


</script>
<main>
    <Nav/>
    <slot />
</main>
<style>
    main{
        display: grid;
        place-items: center;
    }
</style>