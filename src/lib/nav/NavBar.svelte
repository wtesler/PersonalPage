<script>
	import { page } from '$app/stores';
	import Button from '$lib/button/Button.svelte';

	const PATHS = [
		{ name: 'Home', path: '/' },
		{ name: 'About', path: '/about' },
		{ name: 'Portfolio', path: '/portfolio' }
	];

	const onContactClick = () => {
		console.log("CONTACT CLICK");
	}
</script>

<nav class='outer'>
	<div class='first'>
		will tesler.
	</div>
	<div class='center'>
		{#each PATHS as pathObj}
			<a class='link' class:active={$page.url.pathname === pathObj.path} sveltekit:prefetch href={pathObj.path}>
				{pathObj.name}
			</a>
		{/each}
	</div>
	<div class='last'>
		<Button onClick={onContactClick}>
			Contact
		</Button>
	</div>
</nav>

<style>
	.outer {
		width: 100%;
		padding: var(--theme-spacing-7);
		display: flex;
		flex-direction: row;
		position: relative;
		align-items: center;
	}

	.first {
		font-weight: 700;
		font-size: 18px;
	}

	.center {
		display: flex;
		flex-direction: row;
		position: absolute;
		left: 0;
		right: 0;
		align-items: center;
		justify-content: center;
		pointer-events: none;
	}

  @media screen and (max-width: 700px) {
    .center {
			display: none;
    }
  }

	.link {
		padding: 0 1.5px 1px 1.5px;
		margin: 0 var(--theme-spacing-4);
		pointer-events: auto;
		border-bottom: 2px solid transparent;
		text-decoration: none;
		color: black;
		font-weight: 600;
  }

	.link.active {
    border-bottom: 2px solid black;
	}

	.last {
		margin-left: auto;
	}
</style>
