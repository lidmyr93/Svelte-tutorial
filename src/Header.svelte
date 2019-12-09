<script>
  import { Link } from "@c0ldra1n/svero";
</script>

<style>
  header {
    display: flex;
    justify-content: space-between;
    background: rgb(0, 195, 255);
  }
  nav ul {
    display: flex;
    list-style-type: none;
    margin: 0;
  }
  :global(header a) {
    padding: 1em;
    display: block;
    color: white !important;
  }
  :global(.logo) {
    font-weight: bold;
  }
</style>

<header>
  <Link href="/home" className="logo">Hello</Link>

  <nav>
    <ul>
      <li>
        <Link href="/home">Home</Link>
      </li>
      <li>
        <Link href="/about">About</Link>
      </li>
      <li>
        <Link href="/form">Form</Link>
      </li>
      <li>
        <Link href="/datastores">Data Stores</Link>
      </li>
      <li>
        <Link href="/fetchingdata">Fetching Data</Link>
      </li>

    </ul>
  </nav>
</header>
