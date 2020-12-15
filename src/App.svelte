<script>
import Todo from "./components/Todo.svelte";
import Todos from "./components/Todos.svelte";

	 export let name;
</script>

<main>
	<h1>{name}</h1>
	<Todos/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 640px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>