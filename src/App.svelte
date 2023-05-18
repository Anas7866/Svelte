<script>
  import Router from "svelte-spa-router";
  import Home from "./Routes/Home.svelte";
  import About from "./Routes/About.svelte";

  let routes = {
    "/": Home,
    "/about": About,
  };
</script>

<main>
  <Router {routes} />
</main>
