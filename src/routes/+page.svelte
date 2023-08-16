<script>
	import Card from '$components/Card.svelte';
</script>

<div class="wrapper">
	<Card label="Student" src="https://c1.wallpaperflare.com/preview/278/571/763/student-library-books-book.jpg" href="/" />
	<Card label="Uchazeč" src="https://cdn.pixabay.com/photo/2015/09/04/10/42/study-921885_1280.jpg"  href="/" />
	<Card label="Zaměstnanec" src="https://images.pexels.com/photos/8926556/pexels-photo-8926556.jpeg" href="/" />
</div>

<style lang="stylus">
	.wrapper
		display grid
		grid-template-columns repeat(3, 1fr)
		gap 12px
		padding 12px
		padding-top 0

		@media only screen and (max-width 839px)
			grid-template-columns repeat(2, 1fr)

		@media only screen and (max-width 468px)
			grid-template-columns repeat(1, 1fr)
</style>
