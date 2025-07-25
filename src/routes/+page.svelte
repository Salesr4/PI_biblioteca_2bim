<script lang="ts">
    let livro=[
        { 
            id: 1, 
            title: "Destaque 1", 
            imagem:  'https://images.tcdn.com.br/img/img_prod/1271663/a_divina_comedia_capa_dura_461_1_a8c6822358c10562cd9f7c0840cf0653.jpg',
            destaques: true

        },
        { 
            id: 1, 
            title: "Destaque 2", 
            imagem: 'https://m.media-amazon.com/images/I/61iW5sHVzdL._UF1000,1000_QL80_.jpg',
            destaques: true
        },
        { 
            id: 1, 
            title: "Destaque 3", 
            imagem:  'https://m.media-amazon.com/images/I/81D8lw4DSeL._UF350,350_QL50_.jpg',
            destaques: true

        },
        { 
            id: 1, 
            title: "Destaque 4", 
            imagem: 'https://m.media-amazon.com/images/I/61TeYHtBhPL._UF1000,1000_QL80_.jpg',
            destaques: true
        },
        { 
            id: 1, 
            title: "Destaque 5", 
            imagem:  'https://m.media-amazon.com/images/I/91RWiM+C-LL._UF894,1000_QL80_.jpg',
            destaques: true

        },
        { 
            id: 1, 
            title: "Destaque 6", 
            imagem: 'https://m.media-amazon.com/images/I/81Ew3-U+sRL._UF1000,1000_QL80_.jpg',
            destaques: true
        }
    ];
    </script>

<div class="destaques">
    <h1>Destaques</h1>
    <div class="livros flex flex-row justify-around">
        {#each livro as livro}
            {#if livro.destaques}
                <img height="150px" width="100" src={livro.imagem} alt={livro.title}>
            {/if}
        {/each}
    </div>
</div>    