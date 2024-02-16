<script>
    import Child from "./child.svelte";
    let isActive
    let bindText = "red"
    function change(e){
        if(isActive){
            isActive = false
        }
        else{
            isActive = true
        }
        bindText = e.detail.color
    }
</script>

<div class="board-red" class:board-green={isActive}></div>

<p>color: {bindText}</p>
<Child on:changeColor={change}/>

<style>
    .board-red{
        width: 300px;
        height: 300px;

        background-color: red;
    }
    .board-green{
        background-color: green;
    }
</style>