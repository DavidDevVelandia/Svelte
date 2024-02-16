<script>
    import { createEventDispatcher } from 'svelte'
    const dispatch = createEventDispatcher()

    function pulsed(){
        dispatch('isPulsed')
    }
</script>

<button type="button" on:click={pulsed}>Pulsar</button>
