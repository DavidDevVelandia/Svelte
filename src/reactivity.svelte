<script>
    let text = ""
    function handle(e){
        text = e.target.value
    }
</script>

<input type="text" placeholder="put here your name" class="inp" on:keyup={handle}>
<p>{text}</p>
<style>
    .inp{
        margin: 100px 0;
        font-size: 1.6rem;
    }
</style>