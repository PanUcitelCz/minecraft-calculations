<script>
    import test from "../../lib/utils/test"
    let innerWidth = 0;

    $: width = 0;

    console.log(width);
    test()
</script>

<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor rerum veniam a iusto.</p>
<svelte:head>
    <title>Ahoj</title>
</svelte:head>

<svelte:window bind:innerWidth={width} />

<style>
    p{
        background-color: rgba(240, 255, 255, 0);
    }
</style>