<script>
    import NovoComponent from "../NovoComponent.svelte";

    let count = 0;
    $: doubled = count * 2;

    $: if (count >= 1) {
		alert('Esse Titulo não Existe, 51 é pinga!');
		count = 0;
	}

    function increment() {
        count += 1;
    }
    function decrement() {
        count -= 1;
    }

    function zerar() {
        count = 0;
    }
</script>

<div class="container">
    <h1>Contador</h1>
    <button on:click={increment}>+</button>

    <span> {count}</span>

    <button on:click={decrement}>-</button>

    <button on:click={zerar}> zerar </button>

    <p>{count} O dobro é {doubled}</p>
</div>

<style>
    div.container {
        text-align: center;
        background-color: #2c2c2c;
        color: white;
        width: 30%;
        border-radius: 18px;
        padding: 15px;
        margin: auto;
        font-family: "Nunito", sans-serif;
    }

    button{
        color: white;
        border-radius: 10px;
        padding: 10px;
        text-decoration: none;
        border: none;
        background: none;
        cursor: pointer;
        font-size: 50px;
    }

    button:hover {
        color: #FF3E00;
    }

    span{
        text-align: center;
        font-size: 40px;
    }
</style>
