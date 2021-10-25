<script context="module">
	export const prerender = true;
</script>

<script>
	import Hero from '$lib/hero/Hero.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<Hero/>
</section>

<style>
	section {
		width: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
    padding: 0 var(--theme-spacing-7) var(--theme-spacing-7) var(--theme-spacing-7);
  }
</style>
