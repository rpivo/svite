<script lang="ts">
  const world = 'postcss'; // edit world and save to see hmr update
</script>

<style lang="postcss">
  h1 {
    color: orangered; /* change color an save to see hmr update */
    /* you can also use css nesting
    & .world {
      font-size: 2rem;
    }
    */
  }
  .world {
    @apply text-teal-500 italic; /*  here's some tailwind apply */
  }
</style>

<h1 class="border border-current rounded p-4 m-4">
  <!-- tailwind classes in svelte template -->
  
  Hello
  <span class="world">{world}</span>
</h1>
