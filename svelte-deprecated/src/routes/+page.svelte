<script>
  import headerPicture from '../assets/header_picture.jpg';
  import aktu from '../assets/aktu.jpg';
  import aktu2 from '../assets/aktu2.jpg';
  import aktu3 from '../assets/aktu3.jpg';
  import newsPicture from '../assets/newsPicture.jpg';
  import history from '../assets/history.jpg';
  import zavody from '../assets/zavody.jpg';
  import gallery from '../assets/gallery.jpg';
  import plachetnice from '../assets/plachetnice.jpg';
</script>

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
