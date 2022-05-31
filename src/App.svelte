<script>
  import logo from './assets/logo.jpg'
  import './app.css'
</script>

<main>
  <div>
    <img src={logo} alt="YC Logo" />
    <h2>Home</h2>
    Vítejte na stránkách YC Doksy</div>
  <div>
    <h2>Historie</h2>
    <p>
      YACHT CLUB Doksy byl založen roku 1927 …… (nějaký text dodám, vezmeme z nějaké brožury)
    </p>
  </div>

  <div>
    <h2>Závody</h2>
    <table>
      <thead>
        <th>CTL</th>
        <th>Datum</th>
        <th>Počet dní</th>
        <th>Název</th>
        <th>Třídy</th>
      </thead>
      <tbody>
        <tr>
          <td>221704</td>
          <td>23.04.2022</td>
          <td>2</td>
          <td>Optimistický Mácháč</td>
          <td>L,Q</td>
        </tr>
        <tr>
          <td>221705</td>
          <td>14.05.2022</td>
          <td>2</td>
          <td>Mem. Bruno Hámy</td>
          <td>P,Star,F,L</td>
        </tr>
        <tr>
          <td>221706</td>
          <td>21.05.2022</td>
          <td>2</td>
          <td>Sdružený krajský přebor KSJ 16+17</td>
          <td>F,L,P,FB,Star,Q</td>
        </tr>
        <tr>
          <td>221720</td>
          <td>02.07.2022</td>
          <td>4</td>
          <td>Mistrovství ČR v lodní třídě Pirát</td>
          <td>Pirát</td>
        </tr>
        <tr>
          <td>221712</td>
          <td>20.08.2022</td>
          <td>2</td>
          <td>Mácha jezdil Evropu</td>
          <td>Evropa</td>
        </tr>
        <tr>
          <td>221714</td>
          <td>10.09.2022</td>
          <td>2</td>
          <td>Lighthouse Cup</td>
          <td>P,Q,Star,F</td>
        </tr>
      </tbody>
    </table>
  </div>

  <section>
    <h2>Aktuality</h2>
    <article>
      Pro vybraného jedince možnost vkládat a mazat?
    </article>
  </section>

  <section>
    <h2>Galerie</h2>
    <p>Pokud možno více „sekcí“ , kronika, Tour de ostrovy ……</p>
  </section>

  <section>
    <h2>Dokumenty</h2>
    <p>Stanovy, provozní řád, ...</p>
  </section>

  <section>
    <h2>Odkazy</h2>
    <ul>
      <li>ČSJ <a href="www.sailing.cz">www.sailing.cz</a></li>
      <li>Město Doksy <a href="www.doksy.com">www.doksy.com</a></li>
    </ul>
  </section>

  <section>
    <h2>Kontakt</h2>
    <div>
      <p>YACHT CLUB DOKSY
        U jezera 981
        472 01 Doksy
        Telefon loděnice <a href="tel:++420775156852">775 156 852</a>
      </p>
      <p>spolek IČ 48282375
      Nejsme plátci DPH
      účet Moneta a.s. 352300824/0600
      </p>
    </div>
  </section>

  <section>
    <h2>Lidé</h2>
    <div>
      <div>
        <h4>Popper Kamil - předseda</h4>
        <a href="tel:+420777238309">777 238 309</a>
        <a href="mailto:kamilpopper@seznam.cz">kamilpopper@seznam.cz</a>
      </div>
      <div>
        <h4>Kraus Zdeněk - správce</h4>
        <a href="tel:+420724797423">724 797 423</a>
        <a href="mailto:krausdoksy@seznam.cz">krausdoksy@seznam.cz</a>
      </div>
      <div>
        <h4>Šulc Jiří - ekonom</h4>
        <a href="tel:+420777162895">777162895</a>
        <a href="mailto:sulc@thean.cz">sulc@thean.cz</a>
      </div>
      <div>
        <h4>Pokorný Miloslav - mládež a trenéři</h4>
        <a href="tel:+420602174856">602174856</a>
        <a href="mailto:milapokorny@seznam.cz">milapokorny@seznam.cz</a>
      </div>
      <div>
        <h4>Háma Petr ing. - závody a rozhodčí</h4>
        <a href="tel:+420777996728">777 996 728</a>
        <a href="mailto:petr.hama@seznam.cz">petr.hama@seznam.cz</a>
      </div>
      <div>
        <h4>Svobodová Kateřina - členská základna</h4>
        <a href="tel:+420734507228">734 507 228</a>
      </div>
    </div>
  </section>
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  img {
    height: 16rem;
    width: 16rem;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
