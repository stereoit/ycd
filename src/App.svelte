<script>
  import logo from './assets/logo.jpg'
  import './app.css'
  import headerPicture from './assets/header_picture.jpg'
  import aktu from './assets/aktu.jpg';
  import aktu2 from './assets/aktu2.jpg';
  import aktu3 from './assets/aktu3.jpg';
  import newsPicture from './assets/newsPicture.jpg';
  import history from './assets/history.jpg';
  import zavody from './assets/zavody.jpg';
  import gallery from './assets/gallery.jpg';
  import plachetnice from './assets/plachetnice.jpg';

  let isMenuVisible = false

  function toggleMenuCategories() {
    if (isMenuVisible === false) {
      return isMenuVisible = true
    } else return isMenuVisible = false
  }

</script>

<main>

  <section class="flex justify-between w-full px-[20px] lg:px-[400px] mb-[30px]">
    <div class="flex">
      <div class="flex justify-center align-center absolute">
        <img src={logo} class="h-[50px] lg:h-[96px]" alt="YC Logo" />
        <div class="bg-[#ffffff] pr-[15px] h-[50px] lg:h-[96px] lg:flex lg:flex-col lg:justify-center lg:align-center">
          <p class="text-[#c0c003] text-[15px] lg:text-[20px]">YACHT CLUB</p>
          <p class="text-[#2f2874] text-[15px] font-bold lg:text-[25px]">DOKSY</p>
        </div>
      </div>
    </div>

    <nav>
      <ul class="hidden text-[#2f2874] lg:flex">
        <li class="lg:px-[40px] lg:border-r lg:border-[#c0c003] lg:cursor-pointer">AKTUALITY</li>
        <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003] lg:cursor-pointer">HISTORIE</li>
        <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003] lg:cursor-pointer">ZÁVODY</li>
        <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003] lg:cursor-pointer">GALERIE</li>
        <li class="lg:block lg:px-[40px] lg:cursor-pointer">KONTAKTY</li>
      </ul>
      <div class="block text-[#2f2874] lg:hidden">
        {#if isMenuVisible === false}
        <div on:click={toggleMenuCategories}>
          <p class="font-bold">MENU</p>
        </div>
        {:else}
        <div on:click={toggleMenuCategories}>
          <p class="font-bold">MENU</p>
        </div>
        <div class="absolute right-0 w-full mt-[30px] text-center bg-[#ffffff] md:bg-[#ffffff]/[0.5] p-[32px] z-[2]">
          <p>AKTUALITY</p>
          <p class="mt-[5px]">HISTORIE</p>
          <p class="mt-[5px]">ZÁVODY</p>
          <p class="mt-[5px]">GALERIE</p>
          <p class="mt-[5px]">KONTAKTY</p>
        </div>
        {/if}
      </div>
    </nav>
  </section>

  <div class="w-full flex justify-center items-center">
    <div class="absolute text-[#ffffff] text-[25px] lg:text-[50px]">
      <p class="welcome-label">VÍTEJTE NA STRÁNKÁCH</p>
      <p class="welcome-label">YACHT CLUBU DOKSY</p>
    </div>
    <img src={headerPicture} class="w-full" alt="headerPicture"/>
  </div>
  
  <section class="p-[24px] lg:px-[450px]">
    <div class="lg:mt-[40px]">
      <h1 class="text-[#2f2874] font-bold text-[30px] lg:text-[40px] border-b border-[#c0c003]">aktuality</h1>
    </div>
    <div class="mt-[15px] lg:mt-[30px]">
      <div class="py-[8px]">
        <p class="py-[4px] font-light text-[20px]">nějaký datum</p>
        <p class="font-light text-[20px]">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Morbi leo mi, nonummy eget tristique non, rhoncus non leo. Fusce aliquam vestibulum ipsum. Etiam egestas wisi a erat. Morbi imperdiet, mauris ac auctor dictum, nisl ligula egestas nulla, et sollicitudin sem purus in lacus.</p>
      </div>
      <div class="py-[8px]">
        <p class="py-[4px] font-light text-[20px]">nějaký datum</p>
        <p class="font-light text-[20px]">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Morbi leo mi, nonummy eget tristique non, rhoncus non leo. Fusce aliquam vestibulum ipsum. Etiam egestas wisi a erat. Morbi imperdiet, mauris ac auctor dictum, nisl ligula egestas nulla, et sollicitudin sem purus in lacus.</p>
      </div>
      <div class="mt-[8px] overflow-hidden md:flex lg:flex lg:justify-between md:justify-between">
          <img src={aktu} class="border border-[#c0c003] w-full md:w-[300px] lg:w-[320px] md:h-[220px] lg:h-[250px] mb-[10px]" alt="aktu" />
          <img src={aktu2} class="border border-[#c0c003] w-full md:w-[300px] lg:w-[320px] md:h-[220px] lg:h-[250px] mb-[10px]" alt="aktu2" />
          <img src={aktu3} class="border border-[#c0c003] w-full md:w-[300px] lg:w-[320px] md:h-[220px] lg:h-[250px] mb-[10px]" alt="aktu3" />
      </div>
    </div>
  </section>
  
  <img src={newsPicture} class="w-full" alt="news picture" />

  <section class="p-[24px] lg:py-[80px] lg:px-[450px]">
    <div class="md:flex lg:flex md:gap-[30px] lg:gap-[30px]">
      <div class="overflow-hidden shadow-[5px_5px_10px_0_rgba(0,0,0,0.2)] mb-[20px] lg:mb-0 md:h-[450px] md:w-[280px] lg:h-[450px] lg:w-[280px] lg:hover:scale-[1.1]">
        <div>
          <img src={history} class="w-full md:h-[180px] lg:h-[180px]" alt="history"/>
        </div>
        <h1 class="text-[#2f2874] font-medium text-center text-[30px] lg:text-[40px] mt-[20px]">HISTORIE</h1>
        <p class="text-center text-[23px] px-[40px] font-light">Trocha toho čtení o clubu, o nás a yachtingu</p>
        <div class="w-full flex justify-center my-[35px] lg:mb-0">
          <div class="triangle-down" />
        </div>
      </div>
      <div class="overflow-hidden shadow-[5px_5px_10px_0_rgba(0,0,0,0.2)] mb-[20px] lg:mb-0 md:h-[450px] md:w-[280px] lg:h-[450px] lg:w-[280px] lg:hover:scale-[1.1]">
        <div>
          <img src={zavody} class="w-full md:h-[180px] lg:h-[180px]" alt="zavody"/>
        </div>
        <h1 class="text-[#2f2874] font-medium text-center text-[30px] lg:text-[40px] mt-[20px]">ZÁVODY</h1>
        <p class="text-center text-[23px] px-[40px] font-light">Aktuální a přehledný kalendář akcí a závodů</p>
        <div class="w-full flex justify-center my-[35px] lg:mb-0">
          <div class="triangle-down" />
        </div>
      </div>
      <div class="overflow-hidden shadow-[5px_5px_10px_0_rgba(0,0,0,0.2)] mb-[20px] lg:mb-0 md:h-[450px] md:w-[280px] lg:h-[450px] lg:w-[280px] lg:hover:scale-[1.1]">
        <div>
          <img src={gallery} class="w-full md:h-[180px] lg:h-[180px]" alt="gallery"/>
        </div>
        <h1 class="text-[#2f2874] font-medium text-center text-[30px] lg:text-[40px] mt-[20px]">GALERIE</h1>
        <p class="text-center text-[23px] px-[40px] font-light">Fotografie a obrázky ze závodů, klubu a další</p>
        <div class="w-full flex justify-center my-[35px] lg:mb-0">
          <div class="triangle-down" />
        </div>
      </div>
    </div>
  </section>

  <img src={plachetnice} class="w-full" alt="plachetnice"/>

  <footer class="p-[30px] lg:py-[80px] bg-[#2f2874] text-[#ffffff] w-full flex flex-col justify-center items-center">
    <div class="flex flex-col lg:flex-row">
      <h1 class="whitespace-nowrap text-[20px] lg:text-[35px] font-semibold lg:mr-[10px] text-center">YACHT CLUB DOKSY,</h1>
      <p class="text-[20px] lg:text-[35px] font-light text-center">U jezera 981, 472 01 - Doksy</p>
    </div>
    <div>
      <p class="text-[20px] lg:text-[35px] font-light text-center">telefon loděnice: +420 775 156 852</p>
    </div>
    <div class="flex flex-col md:flex-row lg:flex-row py-[30px]">
      <p class="text-[20px] lg:text-[25px] leading-[25px] font-light text-center md:px-[20px] md:border-r md:border-[#ffffff] lg:px-[20px] lg:border-r lg:border-[#ffffff]">Spolek IČ 48282375</p>
      <p class="text-[20px] lg:text-[25px] leading-[25px] font-light text-center md:px-[20px] md:border-r md:border-[#ffffff] lg:px-[20px] lg:border-r lg:border-[#ffffff]">účet: Moneta a.s. 352300824/0600</p>
      <p class="text-[20px] lg:text-[25px] leading-[25px] font-light text-center md:px-[20px] lg:px-[20px]">Nejsme plátci DPH</p>
    </div>

    <hr class="w-full md:w-[40%] md:mb-[50px] md:mt-[30px] lg:w-[30%] mb-[30px] lg:my-[50px] border border-[#c0c003]">

    <div class=" md:grid md:grid-cols-2 md:gap-[35px] lg:grid lg:grid-cols-2 lg:gap-[30px]">
      <div class="lg:p-[10px] lg:flex lg:justify-center lg:items-center lg:flex-col text-center mb-[20px] lg:mb-0">
        <h3 class="text-[20px] lg:text-[25px] font-medium">Popper Kamil - předseda</h3>
        <p class="text-[20px] lg:text-[25px] font-light">+420 777 238 309</p>
        <p class="text-[20px] lg:text-[25px] font-light">kamilpopper@seznam.cz</p>
      </div>
      <div class="lg:p-[10px] lg:flex lg:justify-center lg:items-center lg:flex-col text-center mb-[20px] lg:mb-0">
        <h3 class="text-[20px] lg:text-[25px] font-medium">Kraus Zdeněk - správce</h3>
        <p class="text-[20px] lg:text-[25px] font-light">+420 724 797 423</p>
        <p class="text-[20px] lg:text-[25px] font-light">krausdoksy@seznam.cz</p>
      </div>
      <div class="lg:p-[10px] lg:flex lg:justify-center lg:items-center lg:flex-col text-center mb-[20px] lg:mb-0">
        <h3 class="text-[20px] lg:text-[25px] font-medium">Šulc Jiří - ekonom</h3>
        <p class="text-[20px] lg:text-[25px] font-light">+420 777 162 895</p>
        <p class="text-[20px] lg:text-[25px] font-light">sulc@thean.cz</p>
      </div>
      <div class="lg:p-[10px] lg:flex lg:justify-center lg:items-center lg:flex-col text-center">
        <h3 class="text-[20px] lg:text-[25px] font-medium">Háma Petr ing. - závody a rozhodčí</h3>
        <p class="text-[20px] lg:text-[25px] font-light">+420 777 996 728</p>
        <p class="text-[20px] lg:text-[25px] font-light">petr.hama@seznam.cz</p>
      </div>
    </div>

    <hr class="w-full md:w-[40%] lg:w-[30%] mt-[30px] lg:mt-[50px] border border-[#c0c003]">

    <div class="flex">
      <div class="w-[50px] h-[50px] border border-[#ffffff]">1</div>
      <div class="w-[50px] h-[50px] border border-[#ffffff]">2</div>
      <div class="w-[50px] h-[50px] border border-[#ffffff]">3</div>
    </div>
  </footer>
  <div class="bg-[#ffffff] w-full py-[20px]">
    <p class="text-[15px] lg:text-[25px] font-light text-center">© 2022, Něco a někdo</p>
  </div>

</main>
