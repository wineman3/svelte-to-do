<script>
import Todo from "./Todo.svelte";

	 export let todos = [
     {
       'name': 'test',
       'completed': false,
       'description': 'test'
     }
   ];
</script>

<main>
  <ul>
    {#each todos as i}
      <Todo {...i}> </Todo>
    {/each}
  </ul>
</main>
