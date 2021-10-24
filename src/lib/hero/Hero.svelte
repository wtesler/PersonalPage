<script>

import Button from '$lib/button/Button.svelte';
</script>

<div class='outer'>
	<div class='first'>
		<img class='image' src='public/images/headshot.jpg' alt='Profile Picture'>
	</div>
	<div class='last'>
		<h1 class='heading1'>
			Will Tesler
		</h1>
		<h2 class='heading2'>
			Software Engineer and Web Developer at the forefront of the Modern Web.
		</h2>
		<div class='button'>
			<Button>
				Contact
			</Button>
		</div>
	</div>
</div>

<style>
	.outer {
		width: 100%;
		max-width: 1000px;
		padding: 0 var(--theme-spacing-6) var(--theme-spacing-6) var(--theme-spacing-6);
		display: flex;
		flex-direction: row;
		position: relative;
		align-items: center;
	}

	.first {
		flex: 6;
		padding-right: var(--theme-spacing-5);
	}

	.last {
		flex: 5;
    padding-left: var(--theme-spacing-5);
  }

	.image {
		width: 100%;
		object-fit: cover;
	}

	.heading1 {
		font-size: 54px;
		font-weight: 700;
	}

	.heading2 {
    font-size: 18px;
    font-weight: 400;
		line-height: 28px;
		margin-top: var(--theme-spacing-3);
	}

	.button {
		margin-top: var(--theme-spacing-4);
	}

  @media screen and (max-width: 700px) {
    .outer {
			flex-direction: column;
		}

		.last {
			margin-top: var(--theme-spacing-5);
		}
  }
</style>
