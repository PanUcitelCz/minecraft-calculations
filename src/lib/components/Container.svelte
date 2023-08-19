<script lang="ts">
    interface $$Props {
        variant?: 'regular' | 'card' | 'narrow' | 'table'
    }

    export let variant: $$Props['variant'] = 'regular'
</script>

<div class={variant}>
    <slot />
</div>

<style lang="stylus">
    div
        margin 0 auto
        padding 0 24px
        box-sizing content-box

        @media $small-wide-max
            padding 0 12px

        &.regular
            max-width 1380px
        
        &.table
            max-width 1440px
            padding 0

        &.card
            max-width 965px
        
        &.narrow
            max-width 561px
</style>
