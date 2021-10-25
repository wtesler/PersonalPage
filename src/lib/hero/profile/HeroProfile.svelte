<script>

</script>

<div class='outer'>
	<div class='bg'></div>
	<img class='image' src='images/headshot.png' alt='Profile'>
	<div class='name'>Pro</div>
</div>

<style>
	.outer {
		position: relative;
    --hero-profile-bg-color: #47b6e1FF;
    --hero-profile-bg-shadow: #47b6e188;
  }

	.bg {
		width: 95%;
		height: 90%;
		top: 10%;
		left: 0;
		right: 0;
		margin: 0 auto;
		position: absolute;
		background-color: var(--hero-profile-bg-color);
		border-radius: 200px 200px 0 0;
		box-shadow: 5px 5px 40px 0 var(--hero-profile-bg-shadow);
		border: 5px solid #8ecce7;
		/*border-right: 5px solid #8ecce7;*/
		/*border-left: 5px solid #8ecce7;*/
	}

  .image {
		width: 100%;
		max-width: 350px;
    object-fit: cover;
		position: relative;
		bottom: 5px;
  }

	.name {
    position: absolute;
		transform: rotateZ(-90deg);
		font-weight: 900;
		font-size: 70px;
		top: 50%;
		left: 4%;
		margin: auto 0;
		color: white;
		text-shadow: -5px -5px var(--hero-profile-bg-color);
		user-select: none;
  }
</style>