<script>
import icons from './icons.js'
  export let name;
  export let width = "24";
  export let height = "24";
  let displayIcon = icons[name]
</script>
<svg
class={$$props.class}
{width}
{height}
viewBox="0 0 {displayIcon.box} {displayIcon.box}">{@html displayIcon.svg}</svg>