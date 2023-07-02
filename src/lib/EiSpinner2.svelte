<script>
  export let color = 'currentColor';
  export let size = '50';
  export let role = 'img';
  export let ariaLabel = 'ei spinner 2';
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
  ><circle cx="25" cy="10" r="2" /><circle opacity=".3" cx="25" cy="40" r="2" /><circle
    opacity=".3"
    cx="32.5"
    cy="12"
    r="2"
  /><circle opacity=".3" cx="17.5" cy="38" r="2" /><circle
    opacity=".93"
    cx="17.5"
    cy="12"
    r="2"
  /><circle opacity=".3" cx="32.5" cy="38" r="2" /><circle
    opacity=".65"
    cx="10"
    cy="25"
    r="2"
  /><circle opacity=".3" cx="40" cy="25" r="2" /><circle
    opacity=".86"
    cx="12"
    cy="17.5"
    r="2"
  /><circle opacity=".3" cx="38" cy="32.5" r="2" /><circle
    opacity=".44"
    cx="12"
    cy="32.5"
    r="2"
  /><circle opacity=".3" cx="38" cy="17.5" r="2" /></svg
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
