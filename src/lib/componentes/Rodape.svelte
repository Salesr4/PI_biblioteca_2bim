<main>
  <p>conteúdo main</p>
</main>
<footer class="footer">
  <div class="footer-container">
    <div class="footer-section">
      <h3>Biblioteca</h3>
      <p>frasefrasefrasefrasefrasefrasefrase.</p>
    </div>

    <div class="footer-section">
      <h4>Links</h4>
      <ul>
        <li><a href="/catalogo">Catálogo</a></li>
        <li><a href="/contato">Contato</a></li>
        <li><a href="/sobre">Sobre nós</a></li>
      </ul>
    </div>

    <div class="footer-section">
      <h4>Contato</h4>
      <p>Email: atendimento@biblioteca.com</p>
      <p>Telefone: 8888888888</p>
      <p>Endereço: aaaaaaaaaaaa</p>
    </div>
  </div>
</footer>
<style>

    .footer {
      background-color: #27374D;
      color: #f1f1f1;
      padding: 40px 20px;
      font-family: Arial, sans-serif;
    }

    .footer-container {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: 0 auto;
      gap: 20px;
    }

    .footer-section {
      flex: 1 1 250px;
      min-width: 200px;
    }

.footer-section h3,
.footer-section h4 {
  margin-bottom: 15px;
  color: #DDE6ED;
}

    .footer-section p,
    .footer-section li,
    .footer-section a {
      font-size: 14px;
      line-height: 1.6;
    }

    .footer-section ul {
      list-style: none;
      padding: 0;
      margin: 0;
    }

    .footer-section li {
      margin-bottom: 8px;
    }

    .footer-section a {
      color: #f1f1f1;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .footer-section a:hover {
      color: #DDE6ED;
    }

    @media (max-width: 768px) {
      .footer-container {
        flex-direction: column;
        align-items: center;
        text-align: center;
      }

  .footer-section {
    max-width: 100%;
  }
}

html, body {
  height: 100%;
  margin: 0;
  display: flex;
  flex-direction: column;
}

main {
  flex: 1;
}

</style>

