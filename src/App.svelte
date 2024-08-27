<script>
  import logo from './assets/logo.jpg'
  import './app.css'
  import Contact from './lib/Contact.svelte'
</script>

<main>
  
  <nav>
    <ul>
      <li>Aktuality</li>
      <li>Historie</li>
      <li>Závody</li>
      <li>Galerie</li>
      <li>kontakty</li>
    </ul>
  </nav>

  <section>
    <!-- <h2>Home</h2> -->
    <div class="flex">
      <div class="shrink-0">
        <img src={logo} class="block h-24 w-24" alt="YC Logo" />
      </div>
      <p>Vítejte na stránkách YC Doksy</p>
    </div>
  </section>


  <section class="prose p-6">
    <h2>Historie</h2>
    <p>
      YACHT CLUB Doksy byl založen roku 1927 …… (nějaký text dodám, vezmeme z nějaké brožury)
    </p>
  </section>

  <section class="p-6">
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
  </section>

  <section class="prose p-6">
    <h2>Aktuality</h2>
    <article>
      Pro vybraného jedince možnost vkládat a mazat?
    </article>
  </section>

  <section class="prose p-6">
    <h2>Galerie</h2>
    <p>Pokud možno více „sekcí“ , kronika, Tour de ostrovy ……</p>
  </section>

  <section class="prose p-6">
    <h2>Dokumenty</h2>
    <p>Stanovy, provozní řád, ...</p>
  </section>

  <section class="prose p-6">
    <h2>Odkazy</h2>
    <ul>
      <li>ČSJ <a href="www.sailing.cz">www.sailing.cz</a></li>
      <li>Město Doksy <a href="www.doksy.com">www.doksy.com</a></li>
    </ul>
  </section>

  <section class="prose p-6">
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

  <section class="p-6">
    <h2>Lidé</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4">
      <Contact name="Popper Kamil" title="předseda" tel="777 238 309" email="kamilpopper@seznam.cz" />
      <Contact name="Kraus Zdeněk" title="správce" tel="724 797 423" email="krausdoksy@seznam.cz" />
      <Contact name="Šulc Jiří" title="ekonom" tel="777 162 895" email="sulc@thean.cz" />
      <Contact name="Pokorný Miloslav" title="mládež a trenéři" tel="602 174 856" email="milapokorny@seznam.cz" />
      <Contact name="Háma Petr ing." title="závody a rozhodčí" tel="777 996 728" email="petr.hama@seznam.cz" />
      <Contact name="Svobodová Kateřina" title="členská základna" tel="734 507 228" />
    </div>
  </section>
</main>

<style>
  main {
    background-color: beige;
  }
</style>
