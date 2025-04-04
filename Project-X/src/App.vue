<script>
  
  import { Swiper, SwiperSlide } from 'swiper/vue';

  
  import 'swiper/scss';

  import 'swiper/scss/navigation';

  import 'swiper/scss/pagination';

  
  import { Pagination } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Pagination],
      };
    },
  };

</script>



<template>

  <section class="hero">
    <div id="navbar">
      <a href="#" class="logo">MONTE </a>
        <sanp class="HUA"> HUA </sanp>

        <ul id="nav_list">
          <li class="nav-item">
            <a href="#home">INICIO</a>
          </li>
          <li class="nav-item">
            <a href="#bio"> PORTAL DO CLIENTE</a>
          </li>
          <li class="nav-item">
            <a href="#testimonials">IMÓVEIS</a>
          </li>
          <li class="nav-item">
            <a href="#testimonials">CONTATO</a>
          </li>
        </ul>

        <div class="whats">
            <a href="https://wa.me/5599999999999" target="_blank">
              <i class="fa-brands fa-whatsapp"></i>
            </a>
        </div>

        <div class="hamb">
            <a href="#">
              <i class="fa-solid fa-house"></i>
            </a>
        </div>
      
         
    </div>
  <main class="container">
    <section class="body">
      <div class="background">
        <img src="/fundo 2.jpg" alt="">
      </div>
      <div class="body_page">
        <h1 class="title">MONTE HUA</h1>
        <p class="deslize">Deslize para Aproveitar</p>
      </div>
      </section>
  </main>

  </section>
 
<main class="cont_proc">
    <div class="porc">
      <h2 class="seg_title">Qual imóvel você está buscando?</h2>
        <form class="seleção" action="select">
          <label class="tem" for="marcas">
            <select class="sim" name="caixa_selc" id="slc">
              <option value="1">EMPREENDIMENTO</option>
              <option value="1">MONTE HUA</option>
              <option value="1">GRUPO RAPOM</option>
            </select>

            <select class="sim" name="caixa_selc" id="slc">
              <option value="1">TIPO DE EMPREENDIMENTO</option>
              <option value="1">APARTAMENTO</option>
              <option value="1">CONDOMINIO RESIDENCIAL</option>
              <option value="1">SALA COMERCIAL </option>
              <option value="1">PREDIO COMERCIAL</option>
            </select>

            <select class="sim" name="caixa_selc" id="slc">
              <option value="1">STATUS DO EMPREENDIMENTO</option>
              <option value="1">EM CONSTRUÇÃO</option>
              <option value="1">LAÇAMENTO</option>
              <option value="1">PRONTO PRA MORAR</option>
            </select>

            <select class="sim" name="caixa_selc" id="slc">
              <option value="1">VALOR DO EMPREENDIMENTO</option>
              <option value="1">OPIÇÃO 1- DE 50MIL A 100 MIL</option>
              <option value="1">OPIÇÃO 1- DE 100MIL A 300 MIL</option>
              <option value="1">OPIÇÃO 1- DE 300MIL A 500 MIL</option>
              <option value="1">OPIÇÃO 1- DE 500MIL A 1 MILHÃO</option>
            </select>

          </label>
        </form>
    </div>
</main>

<main class="cont_imo">
    <div class="cont_imoveis">
      <h2 class="til_imo">Imóveis</h2>
      <div class="carousel">
    <swiper
      :slidesPerView="3"
      :spaceBetween="30"
      :pagination="{
        clickable: true,
      }"
      :modules="modules"
      class="mySwiper"
    >
    <swiper-slide><img src="/predio1.jpg" alt="Imagem 1"></swiper-slide>
    <swiper-slide><img src="/predio2.jpg" alt="Imagem 2"></swiper-slide><swiper-slide><img src="/predio6.jpg" alt="Imagem 6"></swiper-slide>
    <swiper-slide><img src="/predio3.jpg" alt="Imagem 3"></swiper-slide><swiper-slide><img src="/predio7.jpg" alt="Imagem 7"></swiper-slide>
    <swiper-slide><img src="/predio4.jpg" alt="Imagem 4"></swiper-slide><swiper-slide><img src="/predio8.webp" alt="Imagem 8"></swiper-slide>
    <swiper-slide><img src="/predio5.jpg" alt="Imagem 5"></swiper-slide><swiper-slide><img src="/predio9.png" alt="Imagem 9"></swiper-slide>
  </swiper>
    <!--<div class="carousel-track">
      <img src="/predio1.jpg" alt="Imagem 1">
      <img src="/predio2.jpg" alt="Imagem 2">
      <img src="/predio3.jpg" alt="Imagem 3">
      <img src="/predio4.jpg" alt="Imagem 4">
      <img src="/predio5.jpg" alt="Imagem 5">
      <img src="/predio6.jpg" alt="Imagem 6">
      <img src="/predio7.jpg" alt="Imagem 7">
      <img src="/predio8.webp" alt="Imagem 8">
      <img src="/predio9.png" alt="Imagem 9">
      <img src="/image10.png" alt="Imagem 10">
    </div>-->
  </div>
    </div>
</main>

<main class="cont_contato">
    <div class="contato">
      <h2 class="til_contato">CONTATO</h2>
      <p class="text">Preencha o formulário para que nossa equipe Possa entrar em contato</p>
      <div class="cadastro">
        <input type="caixa" placeholder="SEU NOME" class="nome">
        <input type="caixa" placeholder="SEU EMAIL" class="email">
        <input type="caixa" placeholder="NUMERO DE CELULAR" class="numero">
        <input type="caixa" placeholder="DIGITE SUA MENSAGEM" class="mensagem">
        <button class="enviar">
          <p>ENVIAR</p>
        </button>
      </div>
    </div>
</main>

<div class="container_final">
    <p class="final">Esse site foite feita para fins de estudo.</p>
</div>
</template>

<style src="/src/scss/style.scss" lang="scss" />
