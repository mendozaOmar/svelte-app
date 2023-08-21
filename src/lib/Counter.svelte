<script lang="ts">
  export let title = "Default Title";
  let count: number = 0
  $: double = count * 2;
  const increment = () => {
    count += 1
  }
</script>

<div id="title" >
  <h2>{title}</h2>
</div>

<button on:click={increment}>
  count is {count} and double is {double}
</button>
