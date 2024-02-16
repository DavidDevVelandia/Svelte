<script>
    import Botonera from "./botonera.svelte";

    let times = 0

    function wasPulsed(){
        console.log('pulsed');
        times++
    }
    function setZero(){
        times = 0
    }
</script>
<p>Me han pulsado {times} {times == 1? 'vez': 'veces'}</p>
<Botonera on:reset={setZero} on:bubbling={wasPulsed}/>