<script lang="ts">
  import type { ToDo } from "./models/todo";

  export let todo: ToDo;
  export let name: string;

  enum CompassDirection {
    North,
    East,
    South,
    West,
  }

</script>

<main>
  <h1>Hello {name}!</h1>
  <p>todo = {CompassDirection.East}</p>
</main>

<style lang="scss">
	@import './scss/variables.scss';

  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: $svelte-red;
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
