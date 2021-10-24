<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/counter/Counter.svelte';
	import Hero from '$lib/hero/Hero.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<Hero/>

	<h2>
		try editing <strong>src/routes/index.svelte</strong>
	</h2>

	<Counter />
</section>

<style>
	section {
		width: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>
