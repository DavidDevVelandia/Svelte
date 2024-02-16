<script>
    import {createEventDispatcher} from 'svelte'
    let change = "red"
    const dispatch = createEventDispatcher()
    function handle(){
        if (change === 'red'){
            change = 'green'
        }else{
            change = 'red'
        }

        dispatch('changeColor', {

            color: change
        })
    }

</script>

<button on:click={handle}>change color</button>

