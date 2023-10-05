<script>
	import PtInputForm from './PTInputForm.svelte';
	import PtToDoList from './PTToDoList.svelte';
</script>

<div class="wrapper">
	<div class="container">
		<PtInputForm />
		<PtToDoList />
	</div>
</div>

<style>
	:global(*) {
		margin: 0;
		padding: 0;
		border: none;
	}
	.wrapper {
		display: grid;
		height: 90vh;
		grid-template-columns: 35vw 30vw 35vw;
		grid-template-rows: 10vh 80vh 10vh;
	}
	.container {
		grid-row-start: 2;
		grid-column-start: 2;
		display: grid;
		grid-template-columns: repeat(20, 5%);
		grid-template-rows: repeat(50, 2%);
		border-radius: 10px;
		background: #e6e6e6;
	}
</style>
