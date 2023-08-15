<script lang="ts">
	export let label: string;
	export let src: string;
</script>

<div class="Card">
	<h2 class="Card-heading">
		{label}
	</h2>
	<img class="Card-image" {src} alt="" />
</div>

<style lang="stylus">
    .Card
        position relative
        min-height 200px
        display flex

        &:after
            position absolute
            inset 0
            content ""
            background green
            opacity .3
            transition opacity .3s ease
        
        &:hover
            &:after
                opacity 0

            .Card-heading
                background green
                top 0
                transform translateY(0)

        &-heading
            position relative
            z-index 1
            color black
            background transparent
            width 100%
            top 50%
            transform translateY(-50%)
            margin 0
            height fit-content
            text-align center
            padding 24px 0
            transition background .3s ease, transform .3s ease, top .3s ease
        
        &-image
            position absolute
            inset 0
            width 100%
            height 100%
</style>
