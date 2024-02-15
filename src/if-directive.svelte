<script>
    let text = "";

    function handle(e){
        text = e.target.value;
    }
</script>
<input type="text" placeholder="text here" on:keyup={handle}>
<button disabled={text === ""}>send message</button>
{#if text !== ""}
    <p class="hideText">{text}</p>
    {:else}
        <p>no content</p>
{/if}

<style>
    .hideText{
        display: block;
        min-width: 2rem;
        width: fit-content;
        height: 3rem;
        background-color: gray;
        color: black;
    }
</style>