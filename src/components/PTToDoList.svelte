<script>
	import PtToDoItem from './PTToDoItem.svelte';

	let items = [
		{
			text: 'ToDo 1',
			isDone: false
		},
		{
			text: 'ToDo 2',
			isDone: false
		},
		{
			text: 'ToDo 3',
			isDone: false
		}
	];
</script>

<div id="todoList" class="todoList">
	{#each items as item}
		<PtToDoItem {...item} />
	{/each}
</div>

<style>
	.todoList {
		grid-area: 9 / 3 / span 34 / span 16;
		display: flex;
		padding: 2vh;
		flex-direction: column;
		background: white;
		border-radius: 10px;
		gap: 2vh;
		overflow: auto;
	}
</style>
