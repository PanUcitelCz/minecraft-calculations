<script>
	import Card from '$components/Card.svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<div class="wrapper">
	<Card label="Student" src="https://dummyimage.com/600x400//" />
	<Card label="Student" src="https://dummyimage.com/600x400//" />
	<Card label="Student" src="https://dummyimage.com/600x400//" />
	<Card label="Student" src="https://dummyimage.com/600x400//" />
	<Card label="Student" src="https://dummyimage.com/600x400//" />
	<Card label="Student" src="https://dummyimage.com/600x400//" />
</div>

<style lang="stylus">
	.wrapper
		display grid
		grid-template-columns repeat(3, 1fr)
		gap 12px
		padding 12px
		padding-top 0
</style>
