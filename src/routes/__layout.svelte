<script>
	import '../app.css';
	import NavBar from '$lib/nav/NavBar.svelte';
</script>

<img class='background' src='images/background.svg' alt='Background' />

<NavBar />

<main class='main'>
	<slot />
</main>

<footer>
</footer>

<style>
	.background {
		width: 100%;
		height: 100vh;
		object-fit: cover;
		position: fixed;
	}

	.main {

	}
</style>
