<script lang="ts">
  import type { HTMLAnchorAttributes } from 'svelte/elements'

  export let href: string
  export let target: HTMLAnchorAttributes['target']
  export let title: HTMLAnchorAttributes['title'] = undefined
</script>

<a class="text-cyan-200 hover:text-cyan-400 hover:border-b border-dotted" {href} {target} {title}><slot /></a>

