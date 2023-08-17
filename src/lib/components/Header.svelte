<script lang="ts">
	let isOpen = false;

	const resize = () => {
		if (window.matchMedia('(min-width: 991px)').matches) {
			isOpen = false;
		}
	};
</script>

<svelte:window on:resize={resize} />

<header class="Header">
	<div class="Header-wrapper">
		<div class="Header-logo">
			<img src="images/logo.svg" alt="" />
		</div>
		<button
			class="Hamburger"
			class:isOpen
			on:click={() => {
				isOpen = !isOpen;
			}}
		>
			<span class="Hamburger-stick" />
			<span class="Hamburger-stick" />
			<span class="Hamburger-stick" />
		</button>
		<nav class="Header-nav" class:isOpen>
			<ul>
				<li><a href="/">Suplování</a></li>
				<li><a href="/">Bakaláři</a></li>
				<li><a href="/">Domov mládeže</a></li>
				<li><a href="/">Školní jídelna</a></li>
				<li><a href="/">O nás</a></li>
				<li><a href="/">Kontakt</a></li>
				<li><a href="/">Výuka na dálku</a></li>
			</ul>
		</nav>
	</div>
</header>

<style lang="stylus">
    .Header
        position relative
        display flex
        justify-content center
        position relative
        width 100%
        height 96px
        background-color #5D5D5D

        &-wrapper
            position relative
            z-index 2
            display flex
            justify-content space-between
            gap 48px
            align-items center
            padding 0 48px
            width 100%
            max-width 1300px

            &:after
                content ""
                position absolute
                z-index 1
                inset 0
                background-color #5D5D5D
                width 50
                height 100%
                left 50%
                transform translateX(-50%)

                @media only screen and (min-width 991px)
                    display none


        &-logo
            position relative
            z-index 4

        &-nav
            position absolute
            z-index 1
            top 0
            left 0
            width 100%
            transform translateY(-100%)
            transition transform .3s ease

            @media only screen and (min-width: 991px)
                position static
                transform none
            
            &.isOpen
                transform translateY(0%)

            ul
                z-index 3
                display flex
                align-items center
                justify-content center
                list-style-type none
                gap 24px
                flex-direction column
                padding-left 0
                margin 0
                padding 24px
                padding-top 96px
                background #5D5D5D

                @media only screen and (min-width: 991px)
                    padding-top 24px
                    display flex
                    flex-direction row
                    justify-content flex-end

                li

                    a
                        text-decoration none
                        color #F7F7F7
                        font-weight bold

                        &:hover
                            text-decoration underline

    .Hamburger
        display block
        position absolute
        z-index 4
        width 35px
        height 25px
        right 35px
        top 35px
        cursor pointer
        z-index 100
        background none
        border none

        @media only screen and (min-width: 991px)
            display none

        &.isOpen
            .Hamburger-stick
                &:nth-child(1)
                    transform: rotate(45deg) translate(8px,8px)

                &:nth-child(2)
                    opacity 0

                &:nth-child(3)
                    transform rotate(-45deg) translate(7px,-7px)

        &-stick
            position absolute
            display flex
            width 100%
            background #F7F7F7
            height 3px
            border-radius 5px
            opacity 1
            transition ease transform 0.3s, ease opacity .3s
            // transform-origin 50% 50%

            &:nth-child(1)
                top 0
            
            &:nth-child(2)
                top 50%
                transform translateY(-50%)

            &:nth-child(3)
                bottom 0
</style>
