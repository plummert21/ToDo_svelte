<script lang="ts">
	export let text: string;
	export let isDone: boolean;
</script>

<div class="todoList__item">
	<div class="todoList__item-info">
		<input class="todoList__item-info-checkbox" type="checkbox" />
		<p class="todoList__item-info-text">{text}</p>
	</div>
	<button class="todoList__item-remove">
		<img src="/img/trash.svg" alt="Удалить" />
	</button>
</div>

<style>
	.todoList__item {
		height: 6vh;
		min-height: 40px;
		display: grid;
		grid-template-columns: repeat(20, 1fr);
		border-radius: 10px;
		background: #ffebeb;
	}

	.todoList__item:hover {
		cursor: pointer;
	}
	/* .todoList__item-done {
		background: #ebffed;
	} */

	.todoList__item-info {
		grid-column: 1 / span 17;
		display: flex;
		align-items: center;
	}

	.todoList__item-info-checkbox {
		margin: 0vw 0.5vw;
	}

	.todoList__item-info-checkbox:hover {
		cursor: pointer;
	}

	/* .todoList__item-done .todoList__item-info-text {
		text-decoration: line-through;
	} */

	.todoList__item-info-text {
		display: flex;
		align-items: center;
		width: 100%;
		font-size: calc(var(--btn-font-size)+0.3vw);
	}

	.todoList__item-remove {
		grid-column: 18 / span 3;
		background-color: transparent;
		border-radius: 0px 10px 10px 0px;
	}

	.todoList__item-remove:hover {
		cursor: pointer;
	}
</style>
