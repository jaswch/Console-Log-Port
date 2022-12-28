<script>
    import { createEventDispatcher } from "svelte";

	const dispatch = createEventDispatcher();
	   
	let text = '';

	function handleInput() {
		dispatch("enter",{
			textToDisplay: text,
		});
	}
</script>

<style>
    input{
		background:rgb(248, 113, 24);
		font-family: 'Courier New', Courier, monospace;
		color: white;
		border: none;
		padding: 8px 50px;
		border-radius: 2px;
	}

	button{
		background:rgb(248, 113, 24);
		font-family: 'Courier New', Courier, monospace;
		color: white;
		border: none;
		padding: 8px 12px;
		border-radius: 2px;
	}

</style>

<input name="enter text to print" bind:value={text}>
<button on:click={handleInput}>Enter</button>

