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
    --hero-profile-bg-color: #e14765FF;
    --hero-profile-bg-shadow: #e1476588;
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
	}

  .image {
		width: 100%;
		max-width: 300px;
    object-fit: cover;
		position: relative;
  }

	.name {
    position: absolute;
		transform: rotateZ(-45deg);
		font-weight: 900;
		font-size: 70px;
		top: 15%;
		left: -5%;
		margin: auto 0;
		color: white;
		text-shadow: -5px -5px var(--hero-profile-bg-color);
		user-select: none;
  }
</style>