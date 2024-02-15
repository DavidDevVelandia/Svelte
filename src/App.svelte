<script>
    import Component from "./component.svelte";
    import Events from "./events.svelte";
    export let name
    let moment = 'tarde'

</script>

<main>
    <h1 class="title">Hola {name}</h1>
    <p>es de {moment}</p>
    <Component nombre = "daniel"/>
    <Events/>
</main>

<style>

    .title{
        font-size: 3rem;
        text-align: center;
        color: red;
    }
    p{
        font-size: 1;
        color: blue;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
</style>