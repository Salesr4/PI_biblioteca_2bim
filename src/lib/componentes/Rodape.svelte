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
      <h4>Contato bla bla</h4>
      <p>Email: atendimento@biblioteca.com</p>
      <p>Telefone: 8888888888</p>
      <p>Endereço: Rua IFRN jsdllda</p>
    </div>
  </div>
</footer>

.footer {
  background-color: #2c3e50;
  color: #ffffff;
  padding: 40px 20px 20px 20px;
  font-family: Arial, sans-serif;
}

.footer-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  max-width: 1200px;
  margin: auto;
}

.footer-section {
  flex: 1;
  min-width: 250px;
  margin: 10px;
}

.footer-section h3, .footer-section h4 {
  margin-bottom: 15px;
  color: #f1c40f;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li {
  margin-bottom: 8px;
}

.footer-section ul li a {
  color: #ecf0f1;
  text-decoration: none;
}

.footer-section ul li a:hover {
  text-decoration: underline;
}

.footer-bottom {
  text-align: center;
  padding-top: 20px;
  border-top: 1px solid #34495e;
  margin-top: 20px;
  font-size: 0.9em;
}
 