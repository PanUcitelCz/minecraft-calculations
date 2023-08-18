<script lang="ts">
    export let text: string;
    export let color: string;
    //export let size: string;
    export let align: String;

</script>


<h1 class={color + " " + align}>
    {text}
</h1>

<style lang="stylus">

    .black
        color black

    .green
        color green
    
    .center
        text-align center
    
    .left
        text-align left

    .right
        text-align right
    


</style>