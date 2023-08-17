<script>
	import Card from '$components/Card.svelte';
</script>

<div class="Hero">
	<h1>Střední odborné učiliště elektrotechnické, Plzeň</h1>
	<h2>Škola doporučena zaměstnavateli</h2>
	<img src="https://plzenskyrozhled.cz/wp-content/uploads/2018/10/soue-plze%C5%88-2-1.png" alt="" />
</div>

<div class="CardWrapper">
	<Card
		label="Student"
		src="https://c1.wallpaperflare.com/preview/278/571/763/student-library-books-book.jpg"
		href="/"
	/>
	<Card
		label="Uchazeč"
		src="https://cdn.pixabay.com/photo/2015/09/04/10/42/study-921885_1280.jpg"
		href="/"
	/>
	<Card
		label="Zaměstnanec"
		src="https://images.pexels.com/photos/8926556/pexels-photo-8926556.jpeg"
		href="/"
	/>
</div>

<div class="Container">
	<h2>Novinky a aktuality</h2>
	<div class="Text">
		<h3>Zahájení školního roku 2023/2024 pro nastupující první ročníky</h3>
		<p>
			Poslední týden v červnu byly nastupujícím žákům odeslány dopisy s formuláři a informacemi
			ohledně zahájení školního roku. Pokud jste dopis neobdrželi, můžete si vše potřebné stáhnout
			zde:
		</p>
	</div>
	<div class="CardWrapper">
		<Card
			label="Obor Telekomunikace"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Obory Mechanik elektrotechnik (všechna zaměření)"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Obor Informační technologie"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Tříleté učební obory"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Denní nástavbové studium"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Dálkové nástavbové studium oborů Provozní technika a Provozní elektrotechnika"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
		<Card
			label="Obor Telekomunikace"
			src="https://c1.wallpaperflare.com/preview/689/175/601/antenna-tower-transmission-communication-telecommunication-cellular.jpg"
			href="/"
		/>
	</div>
	<div class="Text">
		<h3>Jednoleté zkrácené studium oboru Elektrikář</h3>
		<p>
			Datum zahájení záleží na tom, do jaké třídy jste byl(a) zařazen(a). V případě, že jste
			neobdržel(a) dopis s informacemi, kontaktujte nás prosím e-mailem nebo telefonicky (tel. 377
			308 103, e-mail weiszova@souepl.cz)
		</p>
	</div>
</div>

<style lang="stylus">
	.Hero
		position relative
		display flex
		justify-content center
		align-content center
		flex-direction column
		background #9fc334d5
		padding 24px
		margin-bottom 24px
		height 150px
		text-align center
		

		h1, h2
			margin auto
			color white

		h1
			@media only screen and (max-width: 839px)
				font-size 20px

		h2
			@media only screen and (max-width: 839px)
				font-size 15px

		img
			position absolute
			inset 0
			top 0
			z-index -1
			object-fit cover
			width 100%
			height 100%
	
	.CardWrapper
		display grid
		grid-template-columns repeat(1, 1fr)
		gap 12px
		padding-top 0
		position relative
		margin-bottom 24px

		@media only screen and (min-width 420px)
			grid-template-columns repeat(2, 1fr)

		@media only screen and (min-width 991px)
			gap 24px
			grid-template-columns repeat(3, 1fr)


	.Container
		display grid

		h2
			padding 48px 0
			text-align center
			margin 0
		
	.Text
		background-color #5D5D5D
		padding  32px 24px
		margin-bottom 24px
		color white

		h3
			margin 0

		p
			margin 0

</style>
