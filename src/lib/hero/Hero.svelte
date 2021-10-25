<script>
import Button from '$lib/button/Button.svelte';
import HeroProfile from '$lib/hero/profile/HeroProfile.svelte';
</script>

<div class='outer'>
	<div class='first'>
		<div class='profileContainer'>
			<HeroProfile />
		</div>
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
		max-width: 1200px;
		/*padding: 0 var(--theme-spacing-6) var(--theme-spacing-6) var(--theme-spacing-6);*/
		display: flex;
		flex-direction: row;
		position: relative;
		align-items: center;
	}

	.first {
		flex: 5;
		display: flex;
		/*padding-right: var(--theme-spacing-9);*/
	}

	.last {
		flex: 5;
    /*padding-left: var(--theme-spacing-9);*/
  }

	.profileContainer {
		width: 90%;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.heading1 {
		font-size: 54px;
		font-weight: 800;
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

		.first {
			justify-content: center;
		}

		.last {
			margin-top: var(--theme-spacing-5);
		}
  }
</style>
