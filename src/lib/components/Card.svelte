<script lang="ts">

    export let label: string;
    export let src: string;

</script>

<div class="Card">
    <h2>
        {label}
    </h2>
    <img {src} alt="">
</div>

<style lang="stylus">

    .Card
        display grid
        place-items center
        

</style>