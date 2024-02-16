<script>
    function fetch(){
        return new Promise((resolve, reject) => {
            setTimeout(() => {
                resolve({
                    name: "David Velandia",
                    age: 16,
                    job: "programmer"
                })
            }, 3000)
        })
    }
</script>
{#await fetch()}
    <p>Caregando información</p>
{:then APIRequest} 
    <p>name: {APIRequest.name}</p>
    <p>age: {APIRequest.age}</p>
    <p>job: {APIRequest.job}</p>
{/await}