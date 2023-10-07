<script>
	import Footer from "../component/Footer.svelte";
import Nav from "../component/Nav.svelte";


</script>
<main>
    <Nav/>
    <slot />
    <Footer />
</main>
<style>
    main{
        display: grid;
        place-items: center;
    }
</style>