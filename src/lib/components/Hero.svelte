<script lang="ts">
  export let title: string;
  export let text: string;
  export let imageUrl: string;
  export let imageAlt: string;
</script>

<div class="px-6 py-1 pb-10 sm:py-32 lg:px-8">
  <div class="mx-auto max-w-2xl text-center">
    <img class="mx-auto mb-6 w-32 h-32 lg:w-48 lg:h-48 rounded-full" src={imageUrl} alt={imageAlt} />
    <h2 class="text-4xl lg:text-6xl font-bold tracking-tight text-gray-100 sm:text-6x1">{title}</h2>
    <p class="mt-6 text-lg lg:text-xl leading-8 text-gray-300">{text}</p>
  </div>
</div>
