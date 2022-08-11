<script lang="ts">
  import Landing from "./pages/Landing.svelte";
  import {user} from "./store/user.ts";
  import Dashboard from "./pages/Dashboard.svelte";

</script>

<main>
  {#if !$user}
    <Landing />
    {:else}
    <Dashboard />
  {/if}

</main>
