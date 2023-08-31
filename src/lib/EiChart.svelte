<script>
  export let strokeWidth = '2';
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei chart';
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
  ><path d="M18 36h-2V26h-4v10h-2V24h8z" /><path d="M28 36h-2V20h-4v16h-2V18h8z" /><path
    d="M38 36h-2V14h-4v22h-2V12h8z"
  /><path d="M8 36h32v2H8z" /></svg
>

<!--
@component
[Go to docs](https://svelte-evil-icons.vercel.app)
## Props
@prop export let strokeWidth = '2';
@prop export let color = 'currentColor';
@prop export let size = '50';
@prop export let role = 'img';
@prop export let ariaLabel = 'ei chart';
-->
