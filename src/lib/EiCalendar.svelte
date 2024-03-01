<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei calendar';
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
    d="M37 38H13c-1.7 0-3-1.3-3-3V13c0-1.7 1.1-3 2.5-3H14v2h-1.5c-.2 0-.5.4-.5 1v22c0 .6.4 1 1 1h24c.6 0 1-.4 1-1V13c0-.6-.3-1-.5-1H36v-2h1.5c1.4 0 2.5 1.3 2.5 3v22c0 1.7-1.3 3-3 3z"
  /><path d="M17 14c-.6 0-1-.4-1-1V9c0-.6.4-1 1-1s1 .4 1 1v4c0 .6-.4 1-1 1z" /><path
    d="M33 14c-.6 0-1-.4-1-1V9c0-.6.4-1 1-1s1 .4 1 1v4c0 .6-.4 1-1 1z"
  /><path d="M20 10h10v2H20z" /><path d="M12 16h26v2H12z" /><path d="M34 20h2v2h-2z" /><path
    d="M30 20h2v2h-2z"
  /><path d="M26 20h2v2h-2z" /><path d="M22 20h2v2h-2z" /><path d="M18 20h2v2h-2z" /><path
    d="M34 24h2v2h-2z"
  /><path d="M30 24h2v2h-2z" /><path d="M26 24h2v2h-2z" /><path d="M22 24h2v2h-2z" /><path
    d="M18 24h2v2h-2z"
  /><path d="M14 24h2v2h-2z" /><path d="M34 28h2v2h-2z" /><path d="M30 28h2v2h-2z" /><path
    d="M26 28h2v2h-2z"
  /><path d="M22 28h2v2h-2z" /><path d="M18 28h2v2h-2z" /><path d="M14 28h2v2h-2z" /><path
    d="M30 32h2v2h-2z"
  /><path d="M26 32h2v2h-2z" /><path d="M22 32h2v2h-2z" /><path d="M18 32h2v2h-2z" /><path
    d="M14 32h2v2h-2z"
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
@prop export let ariaLabel = 'ei calendar';
-->
