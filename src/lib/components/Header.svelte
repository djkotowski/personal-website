<script lang="ts">
  let { children } = $props();
</script>

<h1 class="text-center text-white text-3xl font-bold mt-20 mb-10">
  {@render children?.()}
</h1>
