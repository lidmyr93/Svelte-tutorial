<script>
  let name = "Jesus";
  let status = false;
</script>

<h1>{name}</h1>
<input bind:value={name} />

<hr />

<label>
  <input type="checkbox" bind:checked={status} />
  Do you want to learn more Svelte?
</label>
<p>
  {#if status}
    Of course I want to learn more Svelte!
  {:else}No I want to keep being a n00b!{/if}
</p>
