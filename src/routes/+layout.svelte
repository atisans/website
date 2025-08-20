<script lang="ts">
  import "../app.css";
  import favicon from "$lib/assets/favicon.svg";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
  <title>The Artisans - Building Tools, Sharing Knowledge</title>
  <meta
    name="description"
    content="Open source, SaaS, and community-driven collaboration for developers worldwide."
  />
</svelte:head>

<main class="min-h-screen bg-offwhite">
  {@render children?.()}
</main>

<!-- Simple Footer -->
<footer class="bg-charcoal text-offwhite py-8">
  <div class="max-w-6xl mx-auto px-4 text-center">
    <div class="flex justify-center items-center mb-4">
      <span class="font-serif text-xl font-bold">The Artisans</span>
    </div>
    <p class="font-sans text-sm text-offwhite/80">
      &copy; {new Date().getFullYear()} The Artisans. All rights reserved.
    </p>
  </div>
</footer>
