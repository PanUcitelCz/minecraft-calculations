<script>
// @ts-nocheck

	import Footer from "$components/Footer.svelte"; //funguje pomocí alias ve svelte.config
    import Header from "$lib/components/Header.svelte";
    import "../lib/css/normallize.css";

</script>



<Header />
<main>
   <slot /> <!--kam se propíše vše ostatní!-->
</main>
<Footer />
<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@10..48,200;10..48,600&display=swap" rel="stylesheet">
</svelte:head>
<style lang="stylus"> 
    //záklaní úprava šablony
    /* your styles go here */

    :global(body)
        font-family 'Bricolage Grotesque', sans-serif

    main
        margin 0 auto
        max-width 1300px

</style>