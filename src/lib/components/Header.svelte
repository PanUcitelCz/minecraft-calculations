<script lang="ts">
	console.log('ahoj');

	import { onMount } from 'svelte';

	let isActive = false;

	onMount(() => {
		const hamburger = document.querySelector('.hamburger');
		const nav = document.querySelector('nav');

		let state = true;

		window.addEventListener('resize', () => {
			if (window.innerWidth < 768) {
				if (hamburger && nav) {
					hamburger.classList.remove('is-active');
					nav.classList.remove('is-active');
				}
			}
		});

		if (hamburger) {
			hamburger.addEventListener('click', () => {
				isActive = !isActive; // Přepnutí hodnoty proměnné isActive
				if (state) {
					if (nav) {
						hamburger.classList.remove('is-active');
						nav.classList.remove('is-active');
					}
					state = false;
				} else {
					if (nav) {
						hamburger.classList.add('is-active');
						nav.classList.add('is-active');
					}
					state = true;
				}
			});
		}
	});

	//TS - deklarace urcit datový typ
</script>

<header>
	<div class="wrapper">
		<div class="logo">
			<img src="https://www.souepl.cz/wp-content/uploads/2022/07/logo_velke_b-3.png" alt="" />
		</div>
		<div class="hamburger {isActive ? 'is-active' : ''}">
			<span class="stick1 stick" />
			<span class="stick2 stick" />
			<span class="stick3 stick" />
		</div>
	</div>
</header>
<div class="wrapper">
    <nav class="nav {isActive ? 'is-active' : ''}">
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
<br>
<br>
<br>



<style lang="stylus">
        
    header
        background-color #5D5D5D
        margin 0
        padding 0
        width 100%
        height 90px
        z-index 10

        .wrapper
            position absolute
            z-index 10
            background-color #5D5D5D
            width 100%
            height 90px
            


            @media only screen and (min-width: 768px)
                position relative

            @media only screen and (min-width: 1300px)
                margin 0 auto
                width 1300px
                
        .logo
            position absolute
            top 5px
            left -20px
            z-index 100

            

            img
                width 65%
                
    .wrapper
        margin 0 auto
        max-width 1300px
    .nav
        position absolute
        top 0
        //right 0
        transition ease transform 0.3s, ease opacity .3s
        transform-origin 50% 50%
        z-index 5
        flex-direction column
        background-color #5D5D5D
        transform translateY(-185px)
        width 100%
        max-width 1300px

        @media only screen and (min-width: 839px)
            transform translateY(30px)
            z-index 15
            background-color rgba(240, 255, 255, 0)
        
        @media only screen and (min-width: 1300px)
            margin 0 auto
            //width 1300px
            display flex
            justify-content center

        &.is-active
                
            padding 15px
            transform translateY(80px)
            //z-index 10
                
        ul
            display flex
            margin 0
            list-style-type none
            gap 24px
            justify-content center
            flex-direction column

            @media only screen and (min-width: 839px)
                display flex
                flex-direction row
                justify-content end
                margin-right 30px

            li

                a
                    text-decoration none
                    color #F7F7F7
                    font-weight bold

                    &:hover
                        text-decoration underline

.hamburger
    width 35px
    position absolute
    height 25px
    right 35px
    top 35px
    cursor pointer
    z-index 100

    @media only screen and (min-width: 839px)
        display none
    
    &.is-active
        .stick1
            transform: rotate(45deg) translate(8px,8px)
        

        .stick2
            opacity 0
        

        .stick3
            transform rotate(-45deg) translate(7px,-7px)       

    .stick
        position absolute
        display flex
        width 100%
        background #F7F7F7
        height 3px
        border-radius 5px
        opacity 1
        transition ease transform 0.3s, ease opacity .3s
        transform-origin 50% 50%

        &.stick1
            top 0
        
        &.stick2
            top 50%
            transform translateY(-50%)

        &.stick3
            bottom 0
        

</style>
