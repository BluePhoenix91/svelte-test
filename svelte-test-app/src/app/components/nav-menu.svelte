<script lang="ts">
  import { Link } from "svelte-navigator";
</script>

<nav class="menu">
  <a href="/">
    <img src="assets/factry-logo-white.png" class="image is-96x96" alt="factry logo"/>
  </a>
  <ul class="menu-list">
    <li>
      <Link to="licenses">Licenses</Link>
    </li>
    <li>
      <Link to="downloads">Downloads</Link>
    </li>
  </ul>
</nav>

<style lang="scss">
  nav {
    background-color: lightgray;

    img {
      height: 80px;
    }
  }
</style>
