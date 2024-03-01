<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei sc skype';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width={size}
  height={size}
  fill={color}
  {role}
  stroke-linecap="round"
  stroke-linejoin="round"
  stroke-width={strokeWidth}
  {...$$restProps}
  aria-label={ariaLabel}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  viewBox="0 0 50 50"
  ><path
    d="M38 27.3c.1-.8.2-1.6.2-2.4 0-1.8-.3-3.5-1-5.1-.7-1.6-1.6-3-2.8-4.2-1.2-1.2-2.6-2.2-4.2-2.8-1.6-.7-3.4-1-5.1-1-.8 0-1.7.1-2.5.2-1.1-.6-2.4-.9-3.7-.9-2.1 0-4.1.8-5.5 2.3-1.5 1.5-2.3 3.4-2.3 5.5 0 1.3.3 2.6 1 3.8-.1.7-.2 1.5-.2 2.3 0 1.8.3 3.5 1 5.1.7 1.6 1.6 3 2.8 4.2 1.2 1.2 2.6 2.2 4.2 2.8 1.6.7 3.4 1 5.1 1 .8 0 1.6-.1 2.3-.2 1.2.7 2.5 1 3.9 1 2.1 0 4.1-.8 5.5-2.3 1.5-1.5 2.3-3.4 2.3-5.5 0-1.3-.3-2.6-1-3.8zM25.1 33c-4.7 0-6.8-2.3-6.8-4 0-.9.7-1.5 1.6-1.5 2 0 1.5 2.9 5.2 2.9 1.9 0 3-1 3-2.1 0-.6-.3-1.4-1.6-1.7l-4.2-1c-3.4-.8-4-2.7-4-4.4 0-3.6 3.3-4.9 6.5-4.9 2.9 0 6.3 1.6 6.3 3.7 0 .9-.8 1.4-1.7 1.4-1.7 0-1.4-2.4-4.9-2.4-1.7 0-2.7.8-2.7 1.9 0 1.1 1.4 1.5 2.5 1.7l3.1.7c3.4.8 4.2 2.7 4.2 4.6.1 2.9-2.1 5.1-6.5 5.1z"
  /></svg
>

<!--
@component
[Go to docs](https://svelte-evil-icons.codewithshin.com)
## Props
@prop export let strokeWidth = ctx.strokeWidth || '2';
@prop export let size = ctx.size || '50';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'ei sc skype';
-->
