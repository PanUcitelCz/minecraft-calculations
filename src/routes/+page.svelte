<script>
    import Card from '$components/Card.svelte'
    import Title from '$components/Title.svelte'
    import BoxText from '$components/BoxText.svelte'
    import Text from '$components/Text.svelte'
    import Container from '$components/Container.svelte'
</script>

<div class="Hero">
    <h1>Střední odborné učiliště elektrotechnické, Plzeň</h1>
    <h2>Škola doporučena zaměstnavateli</h2>
    <img
        src="https://plzenskyrozhled.cz/wp-content/uploads/2018/10/soue-plze%C5%88-2-1.png"
        alt=""
    />
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
    <Title color="black" align="center" text="Novinky a aktuality" />
    <BoxText
        nadpis="Zahájení školního roku 2023/2024 pro nastupující první ročníky"
        text="Poslední týden v červnu byly nastupujícím žákům odeslány dopisy s formuláři a informacemi
		ohledně zahájení školního roku. Pokud jste dopis neobdrželi, můžete si vše potřebné stáhnout
		zde:"
        color="grey"
    />
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
    <Container variant="narrow">
        <!-- <Title size="sm" /> -->
        <Text size="base">
            Datum zahájení záleží na tom, do jaké třídy jste byl(a) zařazen(a). V případě, že jste
            neobdržel(a) dopis s informacemi, kontaktujte nás prosím e-mailem nebo telefonicky (tel. <a
                href="tel:377308103"
            >
                377 308 103
            </a>, e-mail
            <a href="mailto:weiszova@souepl.cz">weiszova@souepl.cz</a>)
        </Text>
    </Container>
    <!-- Title kompnentu udělej podobně jako Text -->
    <!-- Box podobně jako Container -->
    <BoxText
        nadpis="Jednoleté zkrácené studium oboru Elektrikář"
        text="Datum zahájení záleží na tom, do jaké třídy jste byl(a) zařazen(a). V případě, že jste
		neobdržel(a) dopis s informacemi, kontaktujte nás prosím e-mailem nebo telefonicky (tel. 377
		308 103, e-mail weiszova@souepl.cz)"
        color="yellow"
    />

    <BoxText
        nadpis="Soutěž „Drony Plzeňského kraje"
        text="Dne 26. září 2023 proběhne v Střední škole zemědělské a potravinářské, Klatovy, Národních mučedníků 141 soutěž „Drony Plzeňského kraje“.
		Úkolem žáků soutěžních družstev je prolétnout dronem stanovenou dráhu v co nejkratším čase. Do dráhy budou vloženy překážky, kterými musí dron prolétnout či je oblétnout dle vyznačené dráhy.
		Pravidla soutěže budou zveřejněny zde."
        color="grey"
    />

    <BoxText
        nadpis="Informace o termínech maturitních zkoušek v měsíci září 2023"
        text="Žáci obdrží pozvánky na didaktické testy na svůj mail v polovině srpna 2023, DT se budou konat v prvním zářijovém týdnu.
		Praktická zkouška z OV třída ME4 a EI4 v pondělí 11. září 2023 v 7:00 v pracovních oděvech u pana Martina Pihrta (pav. 4, 2. NP).
		
		Praktická zkouška třída IT4 v pondělí 11. září 2023 v 7:45 v učebně B208 Ing. Leba.
		
		Písemná zkouška PN2 v pondělí 11. září 2023 v 7:45 v kanceláři A101 Mgr. Hošková.
		
		Ústní zkoušky čtvrtek 14. září 2023. Rozpisy budou od 1. září 2023 ZDE.
		
		"
        color="grey"
    />
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

		@media only screen and (min-width 420px)
			grid-template-columns repeat(2, 1fr)

		@media only screen and (min-width 991px)
			gap 24px
			grid-template-columns repeat(3, 1fr)


	.Container
		display grid

</style>
