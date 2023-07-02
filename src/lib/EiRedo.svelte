<script>
  export let strokeWidth = '2';
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei redo';
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
    d="M25 38c-7.2 0-13-5.8-13-13s5.8-13 13-13c5.4 0 10.1 3.4 11.9 8.7l-1.9.7c-1.5-4.6-5.4-7.4-10-7.4-6.1 0-11 4.9-11 11s4.9 11 11 11c4.3 0 8.2-2.5 10-6.4l1.8.8C34.7 35 30.1 38 25 38z"
  /><path d="M38 22h-8v-2h6v-6h2z" /></svg
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
