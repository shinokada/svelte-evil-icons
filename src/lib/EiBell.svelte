<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let strokeWidth = ctx.strokeWidth || '2';
  export let size = ctx.size || '50';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'ei bell';
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
    d="M42 36c-6.5 0-7.4-6.3-8.2-11.9C32.9 17.9 32.1 12 25 12s-7.9 5.9-8.8 12.1C15.4 29.7 14.5 36 8 36v-2c4.6 0 5.3-3.9 6.2-10.1.9-6.2 2-13.9 10.8-13.9s9.9 7.7 10.8 13.9C36.7 30.1 37.4 34 42 34v2z"
  /><path d="M25 40c-2.8 0-5-2.2-5-5h2c0 1.7 1.3 3 3 3s3-1.3 3-3h2c0 2.8-2.2 5-5 5z" /><path
    d="M8 34h34v2H8z"
  /><path d="M27 10c0 1.1-.9 1.5-2 1.5s-2-.4-2-1.5.9-2 2-2 2 .9 2 2z" /></svg
>

<!--
@component
[Go to docs](https://svelte-evil-icons.codewithshin.com)
## Props
@prop export let strokeWidth = ctx.strokeWidth || '2';
@prop export let size = ctx.size || '50';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'ei bell';
-->
