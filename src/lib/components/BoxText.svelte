<script lang="ts">
    export let nadpis: string;
    export let color: string;
    export let text: string;
</script>

<div class="Text {color}">
    <h3>{nadpis}</h3>
    <p>
        {text}
    </p>
</div>

<style lang="stylus">

    .Text
        background-color #5D5D5D
        margin 15px 0
        padding 15px
        color white

    .grey
        background-color #5D5D5D

    .yellow
        background-color #E5D429
        color black

</style>