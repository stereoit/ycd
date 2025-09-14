<script>
  import logo from '../assets/logo.jpg'; // Adjusted path
  import '../app.css'; // Assuming app.css is in src for global styles

  let isMenuVisible = false; // Using plain Svelte state

  function toggleMenuCategories() {
    isMenuVisible = !isMenuVisible;
  }
</script>

<header class="flex justify-between w-full px-[20px] lg:px-[400px] mb-[30px]">
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
      <li class="lg:px-[40px] lg:border-r lg:border-[#c0c003]"><a href="/">AKTUALITY</a></li>
      <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003]"><a href="/history">HISTORIE</a></li>
      <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003]"><a href="/zavody">ZÁVODY</a></li>
      <li class="lg:block lg:px-[40px] lg:border-r lg:border-[#c0c003]"><a href="/gallery">GALERIE</a></li>
      <li class="lg:block lg:px-[40px]"><a href="/kontakty">KONTAKTY</a></li>
    </ul>
    <div class="block text-[#2f2874] lg:hidden">
      {#if isMenuVisible === false}
      <div on:click={toggleMenuCategories} role="button" tabindex="0">
        <p class="font-bold">MENU</p>
      </div>
      {:else}
      <div on:click={toggleMenuCategories} role="button" tabindex="0">
        <p class="font-bold">MENU</p>
      </div>
      <div class="absolute right-0 w-full mt-[30px] text-center bg-[#ffffff] md:bg-[#ffffff]/[0.5] p-[32px] z-[2]">
        <p><a href="/">AKTUALITY</a></p>
        <p class="mt-[5px]"><a href="/history">HISTORIE</a></p>
        <p class="mt-[5px]"><a href="/zavody">ZÁVODY</a></p>
        <p class="mt-[5px]"><a href="/gallery">GALERIE</a></p>
        <p class="mt-[5px]"><a href="/kontakty">KONTAKTY</a></p>
      </div>
      {/if}
    </div>
  </nav>
</header>

<main>
  <slot />
</main>

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

<style>
  /* Styles specific to layout could go here if any were in App.svelte's style tag */
  /* For now, assuming app.css covers these, or they are Tailwind classes */
</style>
