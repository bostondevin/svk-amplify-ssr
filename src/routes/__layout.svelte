<script context="module">
  export async function load({ page, fetch, session, context }) {
    return { props: {} };
  }
</script>

<script>
  import { getStores, navigating, page, session } from '$app/stores';
  // import { getStores, navigating } from '$app/stores';
  // import Header from '$lib/Header/index.svelte';
  import '../app.css';
</script>

<main>
  <slot />
</main>

<footer>
  <p>
    visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit
  </p>
</footer>

<style>
  main {
    flex: 1;
    display: flex;
    flex-direction: column;
    padding: 1rem;
    width: 100%;
    max-width: 1024px;
    margin: 0 auto;
    box-sizing: border-box;
  }

  footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px;
  }

  footer a {
    font-weight: bold;
  }

  @media (min-width: 480px) {
    footer {
      padding: 40px 0;
    }
  }
</style>
