<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei trophy';
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
    d="M28.6 29.4c3-2.3 7.4-5.7 7.4-18.4v-1H14v1c0 12.7 4.5 16.1 7.4 18.4 1.7 1.3 2.6 2 2.6 3.6v3c-1.6.2-3.2.8-3.8 2H18c-1.1 0-2 .9-2 2h18c0-1.1-.9-2-2-2h-2.2c-.6-1.2-2.1-1.8-3.8-2v-3c0-1.6.8-2.3 2.6-3.6zm-3.6.5c-.6-.8-1.5-1.5-2.3-2.1-2.7-2.1-6.4-4.9-6.6-15.8h18c-.2 10.8-3.9 13.7-6.6 15.8-1 .7-1.9 1.3-2.5 2.1z"
  /><path d="M18.8 27C18.7 27 8 24.7 8 13v-1h7v2h-5c.6 9.2 9.1 11 9.2 11l-.4 2z" /><path
    d="M31.2 27l-.4-2c.4-.1 8.6-1.9 9.2-11h-5v-2h7v1c0 11.7-10.7 14-10.8 14z"
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
@prop export let ariaLabel = 'ei trophy';
-->
