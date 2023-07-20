<div  class="container" >
    <h1>MEU SITE</h1>

    <ul>
        <li><a href="/contador">Contador</a></li>
        <li><a href="/sobre">sobre</a></li>
    </ul>
</div>

<style>
    div.container {
        display: grid;
        text-align: center;
        background-color: #ccc;
        justify-content: center;
        width: 30%;
        border-radius: 18px;
        padding: 15px;
        margin: auto;
    }
    ul {
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    ul li {
        margin: auto;
        margin: 5px;
    }

    a {
        width: 200px;
        display: block;
        background-color: blue;
        border-radius: 10px;
        padding: 10px;
        text-decoration: none;
        color: white;
        cursor: pointer;
    }

    a:hover {
        background-color: rgb(2, 2, 143);
    }
    h1,
    a {
        text-align: center;
        font-family: "Nunito", sans-serif;
    }
</style>
