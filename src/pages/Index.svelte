<script>
  let bro = "Bro";

  function clickEvent() {
    bro = "Magnus";
    person.status = "Olle";
  }
  let person = {
    status: "Dude"
  };

  let arr = [
    {
      status: "online",
      tagline: "offline"
    },
    {
      status: "uppline",
      tagline: "nerline"
    },
    {
      status: "leftline",
      tagline: "rightline"
    }
  ];
</script>

<h1>Hey {bro}</h1>

<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Amet, mollitia.</p>

<button on:click={clickEvent}>Click here!</button>

{#if person.status === 'Dude'}
  <h1>Hello there</h1>
{:else}
  <h1>{person.status}</h1>
{/if}

<ul>
  {#each arr as { status, tagline }, i}
    <li>
      {i + 1}
      <strong>{status}</strong>
      ({tagline})
    </li>
  {/each}
</ul>
