<script lang="ts">
  import type { HTMLAnchorAttributes } from 'svelte/elements'
  type LinkProps = { children: any, href: string; target: HTMLAnchorAttributes['target']; title?: HTMLAnchorAttributes['title']; rel?: HTMLAnchorAttributes['rel'] }

  let { children, href, target, title, rel }: LinkProps = $props()
</script>

<a class="text-cyan-200 hover:text-cyan-400 hover:border-b border-dotted" {href} {target} {title} {rel}>{@render children?.()}</a>

