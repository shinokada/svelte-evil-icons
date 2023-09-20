<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei star';
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
    d="M15.2 40.6c-.2 0-.4-.1-.6-.2-.4-.3-.5-.7-.4-1.1l3.9-12-10.2-7.5c-.4-.3-.5-.7-.4-1.1s.5-.7 1-.7h12.7L25 5.9c.1-.4.5-.7 1-.7s.8.3 1 .7L30.9 18h12.7c.4 0 .8.2 1 .6s0 .9-.4 1.1L34 27.1l3.9 12c.1.4 0 .9-.4 1.1s-.8.3-1.2 0L26 33l-10.2 7.4c-.2.1-.4.2-.6.2zM26 30.7c.2 0 .4.1.6.2l8.3 6.1-3.2-9.8c-.1-.4 0-.9.4-1.1l8.3-6.1H30.1c-.4 0-.8-.3-1-.7L26 9.5l-3.2 9.8c-.1.4-.5.7-1 .7H11.5l8.3 6.1c.4.3.5.7.4 1.1L17.1 37l8.3-6.1c.2-.1.4-.2.6-.2z"
  /></svg
>

<!--
@component
[Go to docs](https://svelte-evil-icons.vercel.app)
## Props
@prop export let strokeWidth = ctx.strokeWidth || '2';
@prop export let size = ctx.size || '50';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'ei star';
-->
