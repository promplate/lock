<script>
  import "@unocss/reset/tailwind.css";
  import "@fontsource-variable/jetbrains-mono";
  import "uno.css";
</script>

<svelte:head>
  <link rel="icon" href="https://api.iconify.design/noto:package.svg" />
</svelte:head>

<slot />

<style>
  :global(html) {
    --uno: bg-neutral-9 text-white flex flex-col items-center overflow-x-hidden;
  }

  :global(*)::selection {
    --uno: bg-white/15;
  }

  :global(body)::-webkit-scrollbar {
    --uno: bg-neutral-9 w-1 sm-w-1.5 md-w-2 lg-w-2.5 xl-w-3 2xl-w-3.5;
  }

  :global(body)::-webkit-scrollbar-thumb {
    --uno: bg-neutral-7/30 hover-bg-neutral-7/70 rounded-l-sm;
  }

  :global(body *)::-webkit-scrollbar {
    --uno: hidden;
  }
</style>
