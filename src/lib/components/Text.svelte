<script lang="ts">
    // Tadyhlety divný $$Props jsou potřeba aby to fungovalo správně, stejně jako v Reactu.
    // Jde o to že ti pak VSCode našeptává když píšeš komponentu, co tam může/musí být.
    // <Text size="..." />
    // U komponenty při psaní uvozovek ti to nabídne typy.

    interface $$Props {
        // Pokud nemá za jmnénem "?" je props povinnej.
        size: 'xs' | 'sm' | 'base' | 'xl' | 'inherit'
        // Pokud má za jmnénem "?" je props nepovinnej.
        className?: string
        tag?: 'span' | 'p' | 'div' | 'li' | 'b' | 'strong'
    }

    // Pokud bude nepovinnej, a má defaultní hodnotu, ta se tam propíše.
    export let className: $$Props['className'] = undefined
    export let tag: $$Props['tag'] = 'span'
    export let size: $$Props['size'] = 'base'
</script>

<!-- Stuktura (asponň v nějakým základu) by měla vypadat takhle -->
<svelte:element this={tag} class={`Text size-${size} ${className || ''}`}>
    <slot />
</svelte:element>

<style lang="stylus">
    .Text
        // Tady být nemá, můžeš vytvořit samostnout Box komponentu, který ti přídá paddingy a marginy
        // Zároveň ti sem přidám komponentu Container, je jednoduchá, ale taky ukázka jak by mohlo vypadat
        // background-color #5D5D5D
        // margin 15px 0
        // padding 15px
        // color white

    // Barvy taky přes props
    .grey
        background-color #5D5D5D

    .yellow
        background-color #E5D429
        color black
</style>
