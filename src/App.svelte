<script>
  import { Router, Route } from "@c0ldra1n/svero";
  import Header from "./Header.svelte";
  import Index from "./pages/Index.svelte";
  import About from "./pages/About.svelte";
  import Form from "./pages/Form.svelte";
  import DataStores from "./pages/DataStores.svelte";
  import Fetchingdata from "./pages/FetchingData.svelte";
</script>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
  }
  .container {
    width: 80%;
    margin: 4em auto;
  }
</style>

<Header />

<div class="container">
  <Router>
    <Route path="*" component={Index} />
    <Route path="/about" component={About} />
    <Route path="/form" component={Form} />
    <Route path="/datastores" component={DataStores} />
    <Route path="/fetchingdata" component={Fetchingdata} />
  </Router>
</div>
