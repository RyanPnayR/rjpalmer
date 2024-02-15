<script lang="ts">
  import * as Card from "$lib/components/ui/card";
  import { goto } from '$app/navigation';
</script>

<div class="grid place-items-center grid-cols-2 gap-1 h-screen">
<Card.Root on:click={()=>goto('/coder')}>
  <Card.Content>
    <p>Coder</p>
  </Card.Content>
</Card.Root>   
<Card.Root on:click={()=>goto('/comedian')}>
  <Card.Content>
    <p>Comedian</p>
  </Card.Content>
</Card.Root> 
</div>