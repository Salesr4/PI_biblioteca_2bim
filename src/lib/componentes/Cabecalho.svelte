<div id="cabecalho">
    <div>
        <img src="./logo.png" alt="">
    </div>
    <div>
        <input type="search" name="busca-livro" id="busca-livro" placeholder="Buscar livro...🔍">
    </div>
    <nav>
        <ul>
            <li><a href="/inicio">Início</a></li>
            <li><a href="/catalogo">Catalogo</a></li>
            <li><a href="/sobre">Sobre</a></li>
            <li><a href="/contato">Contato</a></li>
        </ul>
    </nav>
</div>
<style>
    #cabecalho {
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: #27374D;
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
        gap: 4rem; /* Adiciona espaçamento entre os itens */
    }
    li {
        color: #f5f5f5;
        font-size: 1.2rem;
    }

    img{
        width: 120px;
        height: auto;
        display: block;
    }

    #busca-livro {
        width: 200%;
        height: 3rem;
        border-radius: 0.5rem;
        padding: 0.5rem;
        border: 1px solid #ccc;
        color: #f5f5f5;
    }
</style>
