<script>
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei credit card';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width={size}
  height={size}
  fill={color}
  {role}
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
    d="M39 38H11c-1.7 0-3-1.3-3-3V15c0-1.7 1.3-3 3-3h28c1.7 0 3 1.3 3 3v20c0 1.7-1.3 3-3 3zM11 14c-.6 0-1 .4-1 1v20c0 .6.4 1 1 1h28c.6 0 1-.4 1-1V15c0-.6-.4-1-1-1H11z"
  /><path d="M9 16h32v6H9z" /><path d="M12 26h1v2h-1z" /><path d="M14 26h1v2h-1z" /><path
    d="M16 26h1v2h-1z"
  /><path d="M19 26h1v2h-1z" /><path d="M21 26h1v2h-1z" /><path d="M23 26h1v2h-1z" /><path
    d="M26 26h1v2h-1z"
  /><path d="M28 26h1v2h-1z" /><path d="M30 26h1v2h-1z" /><path d="M33 26h1v2h-1z" /><path
    d="M35 26h1v2h-1z"
  /><path d="M37 26h1v2h-1z" /></svg
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
