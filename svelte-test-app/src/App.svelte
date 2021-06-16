<script lang="ts">
  import { Router, Route } from "svelte-navigator";
  import Breadcrumbs from "./app/components/breadcrumbs.svelte";
  import NavMenu from "./app/components/nav-menu.svelte";
  import Historian from "./app/pages/download/historian.svelte";
  import Licenses from "./app/pages/licenses/licenses.svelte";
</script>

<main>
  <Router>
    <NavMenu />
    <Breadcrumbs />
    <Route path="downloads" component={Historian} />
    <Route path="licenses" components={Licenses} />
  </Router>
</main>

<style global lang="scss">
  @import "./scss/_base.scss";
</style>
