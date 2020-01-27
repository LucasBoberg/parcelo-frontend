<style>
  footer {
    height: 280px;
    background-color: #000;
    position: relative;
  }
  .wrapper {
    padding: 3rem 8vw;
    color: #FFF;
    display: grid;
    grid-template-columns: 18% 20% 20% auto;
  }
  h1 {
    font-size: 3rem;
    font-weight: 600;
  }
  ul {
    list-style: none;
  }
  .list-header {
    font-size: 1.1rem;
    margin-bottom: 0.4rem;
  }
  a {
    text-decoration: none;
  }
  .footer-image {
    position: absolute;
    right: 0;
    top: 0;
  }

  @media screen and (max-width: 1024px) {
    .wrapper {
      grid-template-columns: auto auto auto auto;
    }
    .footer-image {
      display: none;
    }
  }
  @media screen and (max-width: 640px) {
    .wrapper {
      grid-template-columns: auto;
      padding-bottom: 0;
    }
    footer {
      height: auto;
    }
    h1 {
      font-size: 2rem;
      width: 100%;
      text-align: center;
    }
    ul {
      padding: 0;
      width: 100%;
      text-align: center;
    }
  }
</style>

<footer>
  <div class="wrapper">
    <h1>Parcelo</h1>
    <ul>
      <li class="list-header">FÖRETAG</li>
      <li><a target="_blank" rel="noopener" href="/cookies">Cookies</a></li>
      <li><a target="_blank" rel="noopener" href="/terms">Användarvillkor</a></li>
    </ul>
    <ul>
      <li class="list-header">SOCIALA MEDIER</li>
      <li><a target="_blank" rel="noopener" href="https://www.instagram.com/parcelouf/">Instagram</a></li>
    </ul>
    <ul>
      <li class="list-header">KONTAKT</li>
      <li><a target="_blank" rel="noopener" href="mailto:kontakt@parcelo.se">kontakt@parcelo.se</a></li>
    </ul>
  </div>
  <img class="footer-image" alt="footer image" src="footer.svg"/>
</footer>