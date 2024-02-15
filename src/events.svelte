<script>
    export let variable = 0;
    const sum = () => {
        variable += 1
    }
</script>
<button on:click={sum}>
    <p>{variable}</p>
    click
</button>