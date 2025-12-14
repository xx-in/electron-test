<script lang="ts">
  import Router from "svelte-spa-router";
  import Home from "./routes/Home.svelte";
  import About from "./routes/About.svelte";

  const routes = {
    "/": Home,
    "/about": About,
  };
</script>

<svelte:head>
  <title>electron svelte template</title>
</svelte:head>

<a href="#/">home</a>
<a href="#/about">about</a>
<Router {routes}></Router>
