<script lang="ts">
  import Button, {Label} from '@smui/button'

  let count: number = 0
  const increment = () => {
    count += 1
  }
</script>

<Button color="secondary" on:click={increment} variant="unelevated">
  count is {count}
</Button>
