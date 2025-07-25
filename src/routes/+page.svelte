<script lang="ts">
    let livro=[
        { 
            id: 1, 
            title: "A divina comédia", 
            imagem:  'https://images.tcdn.com.br/img/img_prod/1271663/a_divina_comedia_capa_dura_461_1_a8c6822358c10562cd9f7c0840cf0653.jpg',
            destaques: true,
            autor: "Machado de Assis",
            fotoAutor: 'https://riomemorias.com.br/wp-content/uploads/2025/02/Captura-de-Tela-2025-02-10-as-06.41.44-1-791x1024.png'
        },
        { 
            id: 2, 
            title: "A República", 
            imagem: 'https://m.media-amazon.com/images/I/61iW5sHVzdL._UF1000,1000_QL80_.jpg',
            destaques: true,
            autor: "Itamar Vieira Junior",
            fotoAutor: 'https://flitabira.com.br/wp-content/uploads/2024/09/Itamar-Vieira-Junior.jpg'
        },
        { 
            id: 3, 
            title: "O estranho misterioso", 
            imagem:  'https://m.media-amazon.com/images/I/81D8lw4DSeL._UF350,350_QL50_.jpg',
            destaques: true,
            autor: "Clarice Lispector",
            fotoAutor: 'https://s2.static.brasilescola.uol.com.br/be/2022/09/clarice-lispector.jpg'
        },
        { 
            id: 4, 
            title: "O manifesto comunista", 
            imagem: 'https://m.media-amazon.com/images/I/61TeYHtBhPL._UF1000,1000_QL80_.jpg',
            destaques: true,
            autor: "Jorge Amado",
            fotoAutor: 'https://uploads.metroimg.com/wp-content/uploads/2018/12/31124916/jorgeamado1.193102.jpg'
        },
        { 
            id: 5, 
            title: "Memorias postumas de Brás Cubas", 
            imagem:  'https://m.media-amazon.com/images/I/91RWiM+C-LL._UF894,1000_QL80_.jpg',
            destaques: true,
            autor: "Martin Luther King Jr.",
            fotoAutor:'https://static.todamateria.com.br/upload/ma/rt/martinlutherking-cke.jpg'
        },
        { 
            id: 6, 
            title: "Quarto de despejo", 
            imagem: 'https://m.media-amazon.com/images/I/81Ew3-U+sRL._UF1000,1000_QL80_.jpg',
            destaques: true,
            autor: "Dan Brown",
            fotoAutor: 'https://images-na.ssl-images-amazon.com/images/S/amzn-author-media-prod/ulmb4n9uvsd27upr84d0gcp2dp.jpg'
        }
    ];
</script>

<style>
    .livros-box {
        background: #526D82;
        border-radius: 20px;
        box-shadow: 0 2px 12px rgba(0,0,0,0.12);
        padding: 20px 24px;
        margin-bottom: 40px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .livros-row {
        display: flex;
        flex-direction: row;
        justify-content: center;
        gap: 30px;
        flex-wrap: wrap;
        align-items: center;
    }
    .livro-col {
        display: flex;
        flex-direction: column;
        align-items: center;
        background: transparent;
        padding: 0;
        border-radius: 0;
        box-shadow: none;
        min-width: 0;
    }
    .autores-box {
        background: #9DB2BF;
        border-radius: 18px;
        box-shadow: 0 2px 12px rgba(0,0,0,0.12);
        padding: 32px 24px;
        margin-bottom: 40px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .autores-row {
        display: flex;
        flex-direction: row;
        justify-content: center;
        gap: 30px;
        flex-wrap: wrap;
        align-items: center;
    }
    .autor-col {
        display: flex;
        flex-direction: column;
        align-items: center;
        background: transparent;
        padding: 0;
        border-radius: 0;
        box-shadow: none;
        min-width: 0;
    }
    .img-autor {
        width: 180px;
        height: 180px;
        object-fit: cover;
        border-radius: 8px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.15);
        margin-bottom: 8px;
    }
    .destaque-titulo {
        color: #fff;
        background: #27374D;
        padding: 8px 24px;
        border-radius: 12px;
        font-weight: bold;
        font-size: 2rem;
        text-align: center;
        margin-bottom: 24px;
        letter-spacing: 1px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.10);
        display: inline-block;
    }
    .autores-titulo {
        color: #fff;
        background: #27374D;
        padding: 8px 24px;
        border-radius: 12px;
        font-weight: bold;
        font-size: 2rem;
        text-align: center;
        margin-bottom: 24px;
        letter-spacing: 1px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.10);
        display: inline-block;
    }
</style>

<div class="destaques">
    <div class="livros-box">
        <h1 class="destaque-titulo">Destaques</h1>
        <div class="livros-row">
            {#each livro as livro}
                {#if livro.destaques}
                    <div class="livro-col">
                        <img height="150px" width="200" src={livro.imagem} alt={livro.title}>
                        <h2>{livro.title}</h2>
                    </div>
                {/if}
            {/each}
        </div>
    </div>
    <div class="autores-box">
        <h1 class="autores-titulo">Autores em Destaque</h1>
        <div class="autores-row">
            {#each livro as livro}
                {#if livro.destaques}
                    <div class="autor-col">
                        <img class="img-autor" src={livro.fotoAutor} alt={livro.autor}/>
                        <h2>{livro.autor}</h2>
                    </div>
                {/if}
            {/each}
        </div>
    </div>
</div>