<div id="cabecalho">
    <div>
        <h1>logo do Cabeçalho</h1>
    </div>
    <div>
    </div>
    <nav>
        <ul>
            <li><a href="/">inicio</a></li>
            <li><a href="/sobre">sobre</a></li>
            <li><a href="/contato">contato</a></li>
        </ul>
    </nav>
</div>
<style>
    #cabecalho {
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: rgba(87, 87, 248, 0.705);
        padding: 1rem;
        border-bottom: 1px solid;
        width: 100%;
    }

    ul {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        list-style-type: none;
        width: 100%;
        gap: 2rem; /* Adiciona espaçamento entre os itens */
    }
</style>
