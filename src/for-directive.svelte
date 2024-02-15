<script>
    let elements = 
    [
        { id: '103181', name: 'Buy potato', finished: false},
        { id: '124098', name: 'Clean garden', finished: true},
        { id: '937463', name: 'Send mail', finished: true},
        { id: '203918', name: 'call to Lucia', finished: false}
    ]
</script>

{#each elements as e, index (e.id)}
    {#if e.finished == false}
        <p>{e.name}</p>
    {:else}
        <p class="scratched">{e.name}</p>
    {/if}
{/each}

<style>
    .scratched{
        text-decoration:line-through;
    }
    .scratched::after{
        content: '✔️';
    }
</style>