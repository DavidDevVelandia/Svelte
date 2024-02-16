<script>
    import Component from "./component.svelte";
    import Events from "./events.svelte";
    import Reactivity from "./reactivity.svelte";
    import IfDirective from "./if-directive.svelte";
    import ForDirective from "./for-directive.svelte";
    import AwaitDirective from "./await-directive.svelte";
    import Binding from "./binding.svelte";
    import Parent from "./custom-event/parent.svelte";
    import Container from "./events-bubbling/container.svelte";
    export let name
    let moment = 'tarde'

</script>

<main>
    <h1 class="title">Hola {name}</h1>
    <p>es de {moment}</p>
    <Component nombre = "daniel"/>
    <Events/>
    <Reactivity/>
    <IfDirective/>
    <ForDirective/>
    <AwaitDirective/>
    <Binding/>
    <br>
    <Parent/>
    <br>
    <Container/>
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