<script>
    let name = "David"
    let input
    function handle(){
        
        console.log(input.value)
    }
</script>

<p>Tu nombre es {name}</p>
<p><input type="text" bind:value={name} bind:this={input} on:keyup={handle}></p>
