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
    grid-template-columns: 20% auto;
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

  @media screen and (max-width: 992px) {
    .wrapper {
      grid-template-columns: auto auto;
    }
    .footer-image {
      display: none;
    }
  }
  @media screen and (max-width: 340px) {
    .wrapper {
      grid-template-columns: 40% auto;
    }
    h1 {
      font-size: 2rem;
    }
  }
</style>

<footer>
  <div class="wrapper">
    <h1>Parcelo</h1>
    <ul>
      <li class="list-header">SOCIALA MEDIER</li>
      <li><a target="_blank" rel="noopener" href="https://www.instagram.com/parcelouf/">Instagram</a></li>
    </ul>
  </div>
  <img class="footer-image" alt="footer image" src="footer.svg"/>
</footer>