<form class="form_input">
	<input class="form_input__text" />
	<button class="form_input__btn">Добавить</button>
</form>

<style>
	.form_input {
		grid-area: 4 / 3 / span 3 / span 16;
		display: grid;
		grid-template-columns: repeat(10, 10%);
	}

	.form_input__text {
		grid-column: 1 / span 7;
		padding: 0.5vw;
		font-size: 2.2vh;
		border-radius: 10px 0px 0px 10px;
	}

	.form_input__btn {
		grid-column: 8 / span 3;
		font-size: var(--btn-font-size);
		border-radius: 0px 10px 10px 0px;
		background: #fbcc28;
	}
</style>
