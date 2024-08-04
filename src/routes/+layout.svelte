<script>
  import { base } from '$app/paths';
</script>

<div class="layout">
  <header>
    <h1>Welcome to SvelteKit</h1>
    <nav>
      <a href="{base}/">Home</a>
      <a href="{base}/about">About</a>
    </nav>
    <p>
      Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
    </p>
  </header>
  <section class="spa">Single Page App with routing!!!</section>
  <main>
    <slot />
  </main>
  <footer>by uniboxx</footer>
</div>

<style>
  * {
    box-sizing: border-box;
  }
  .layout {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    min-height: 100svh;
    padding: 2rem;
  }
  nav {
    display: flex;
    justify-content: center;
    gap: 2rem;
  }
  nav a {
    text-decoration: none;
    color: blue;
    font-size: 1.2rem;
    border: 1px solid purple;
    padding: 0.5rem 1rem;
    border-radius: 10px;
    outline: 1px solid rosybrown;
    outline-offset: 2px;
    transition: 0.5s;
  }
  nav a:hover {
    background: #eee;
  }
  .spa {
    font-size: 1.3rem;
    color: green;
    background-color: rgba(0, 128, 0, 0.2);
    padding: 0.3rem 0.6rem;
    border-radius: 10px;
  }
  main {
    flex: 1;
  }
  footer {
    display: flex;
    align-self: end;
    font-size: 1.2rem;
  }
</style>
