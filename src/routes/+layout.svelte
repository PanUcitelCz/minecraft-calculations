<script>
	import Footer from "$components/Footer.svelte"; //funguje pomocí alias ve svelte.config
    import Header from "$lib/components/Header.svelte";
    import "../lib/css/normallize.css";

</script>

<Header />
<main>
   <slot /> <!--kam se propíše vše ostatní!-->
</main>
<Footer />

<style lang="stylus"> 
    //záklaní úprava šablony
    /* your styles go here */

    main
        margin 0 auto
        max-width 1300px

</style>