<script lang="ts">
  type Props = {
    children?: any
    title: string
    imageUrl: string
    imageAlt: string
  };
  let { children, title, imageUrl, imageAlt }: Props = $props()
</script>

<div class="px-6 py-1 pb-10 sm:pt-32 sm:pb-24 lg:px-8">
  <div class="mx-auto max-w-2xl text-center">
    <img class="mx-auto mb-6 w-32 h-32 lg:w-48 lg:h-48 rounded-full" src={imageUrl} alt={imageAlt} />
    <h2 class="text-4xl lg:text-6xl font-bold tracking-tight text-gray-100 sm:text-6x1">{title}</h2>
    {@render children?.()}
  </div>
</div>
