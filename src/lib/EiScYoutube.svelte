<script>
  export let strokeWidth = '2';
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei sc youtube';
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
    d="M39.7 18.6s-.3-2.1-1.2-3c-1.1-1.2-2.4-1.2-3-1.3C31.3 14 25 14 25 14s-6.3 0-10.5.3c-.6.1-1.9.1-3 1.3-.9.9-1.2 3-1.2 3S10 21 10 23.4v2.2c0 2.4.3 4.9.3 4.9s.3 2.1 1.2 3c1.1 1.2 2.6 1.2 3.3 1.3 2.4.1 10.2.2 10.2.2s6.3 0 10.5-.3c.6-.1 1.9-.1 3-1.3.9-.9 1.2-3 1.2-3s.3-2.4.3-4.8v-2.2c0-2.4-.3-4.8-.3-4.8zm-17.8 9.8V20l8.1 4.2-8.1 4.2z"
  /></svg
>
<!--
@component
[Go to Document](https://shinokada.github.io/svelte-cssgg-icons/)
## Props
@prop role = 'img';
@prop size = '50';
@prop color = 'currentColor'
@prop ariaLabel='file name'
## Event
- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout
-->
