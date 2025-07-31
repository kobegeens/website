<script>
    import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";
    import "$lib/assets/app.css";
    import { fly } from 'svelte/transition'

    export let data
</script>

<Navbar />

<svelte:head>
    <title>𝗞𝗼𝗯𝗲 𝗚𝗲𝗲𝗻𝘀</title>
</svelte:head>

<main>
{#key data.url}
  <div
    in:fly={{ x: -200, duration: 300, delay: 300 }}
    out:fly={{ x: 200, duration: 300 }}
  >
    <slot />
  </div>
{/key}
</main>

<Footer />