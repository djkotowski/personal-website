<script lang="ts">
  import type { HTMLAnchorAttributes } from 'svelte/elements'

  export let href: string
  export let target: HTMLAnchorAttributes['target']
</script>

<a class="text-cyan-200 hover:text-cyan-400 hover:border-b border-dotted" {href} {target}><slot /></a>

