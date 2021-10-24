<script>
	export let onClick;
</script>
<div class='button' on:click={onClick}>
	<slot />
</div>
<style>
  .button {
		display: table;
    background-color: #4531c5;
    color: #fff;
    border-radius: 5px;
    padding: var(--theme-spacing-3) var(--theme-spacing-4);
		cursor: pointer;
		user-select: none;
		font-size: 16px;
		transition: background-color .25s;
  }

	.button:hover {
    background-color: #332594;
	}
</style>