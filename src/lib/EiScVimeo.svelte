<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei sc vimeo';
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
    d="M38 19.6c-.1 2.7-2 6.4-5.6 11.1-3.8 4.9-7 7.4-9.6 7.4-1.6 0-3-1.5-4.1-4.5-.7-2.7-1.5-5.5-2.2-8.2-.8-3-1.7-4.5-2.7-4.5-.2 0-.9.4-2.2 1.3l-1.3-1.7c1.4-1.2 2.7-2.4 4-3.6 1.8-1.6 3.2-2.4 4.1-2.5 2.2-.2 3.5 1.3 4 4.4.5 3.4.9 5.5 1.1 6.4.6 2.8 1.3 4.2 2.1 4.2.6 0 1.5-.9 2.6-2.8 1.2-1.8 1.8-3.2 1.9-4.2.2-1.6-.5-2.4-1.9-2.4-.7 0-1.3.2-2 .5 1.4-4.5 4-6.6 7.8-6.5 2.8.1 4.2 1.9 4 5.6z"
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
@prop export let ariaLabel = 'ei sc vimeo';
-->
