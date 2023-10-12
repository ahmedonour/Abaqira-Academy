<script>
    export let Heading;
    export let Desc;
</script>
<main>
    <h1>{Heading}</h1>
    <p>{Desc}</p>
    <p><i>Empowering Minds, Enriching Lives.</i></p>
    <button>Join Us Now</button>
</main>
<style>
    main{
        width: 80vw
    }
    button{
        border-radius: 20px;
background: var(--Contact-bg, #384CFF);
        border: none;
        color: #fff;
        padding: 1rem 2rem;
        border-radius: 15px;
        font-weight: 800;
        font-size: 1rem;
        font-family: var(--ff-Open-Sans);
    }
</style>