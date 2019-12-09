<script>
  import { onDestroy } from "svelte";
  import { status } from "../stores.js";

  let the_status;

  const stat = status.subscribe(val => {
    the_status = val;
  });

  function changeStore() {
    status.update(n => (n = "bro"));
  }
  onDestroy(stat);
</script>

<h1 on:mouseover={changeStore}>{the_status}</h1>
