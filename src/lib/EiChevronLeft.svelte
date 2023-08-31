<script>
  export let strokeWidth = '2';
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei chevron left';
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
  viewBox="0 0 50 50"><path d="M27.3 34.7L17.6 25l9.7-9.7 1.4 1.4-8.3 8.3 8.3 8.3z" /></svg
>

<!--
@component
[Go to docs](https://svelte-evil-icons.vercel.app)
## Props
@prop export let strokeWidth = '2';
@prop export let color = 'currentColor';
@prop export let size = '50';
@prop export let role = 'img';
@prop export let ariaLabel = 'ei chevron left';
-->
