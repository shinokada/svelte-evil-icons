<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei retweet';
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
  ><path d="M38 35h-2V17c0-.6-.4-1-1-1H18v-2h17c1.7 0 3 1.3 3 3v18z" /><path
    d="M37 36.5l-6.8-7.8 1.6-1.4 5.2 6.2 5.2-6.2 1.6 1.4z"
  /><path d="M32 36H15c-1.7 0-3-1.3-3-3V15h2v18c0 .6.4 1 1 1h17v2z" /><path
    d="M18.2 22.7L13 16.5l-5.2 6.2-1.6-1.4 6.8-7.8 6.8 7.8z"
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
@prop export let ariaLabel = 'ei retweet';
-->
