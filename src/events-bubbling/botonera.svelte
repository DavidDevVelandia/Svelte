<script>
    import Button from "./button.svelte"
    import { createEventDispatcher} from 'svelte'
    let dispatch = createEventDispatcher()
    function reset(){
        dispatch('reset')
    }
    function bubblingFun(){
        dispatch('bubbling')
    }

</script>

<button type="button" on:click={reset}>Reiniciar</button>
<Button on:isPulsed={bubblingFun}/>
