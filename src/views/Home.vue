<template>
  <div class="home">
    <Carousel />

    <section class="container my-4">
      <div class="row m-0">
        <div class="position-relative col-6">
          <a href="/ie/outlet/womens/">
            <picture
              ><source srcset="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C1-Mobile.jpg" media="(max-width: 768px)" />
              <img src="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C1-Desktop.jpg" alt="Shop Women's" class="w-100" />
            </picture>
            <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
              <button type="button" class="btn btn-primary">Women's</button>
            </div>
          </a>
        </div>
        <div class="position-relative col-6">
          <a href="/ie/outlet/mens/">
            <picture
              ><source srcset="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C2-Mobile.jpg" media="(max-width: 768px)" />
              <img src="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C2-Desktop.jpg" alt="Shop Women's" class="w-100" />
            </picture>
            <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
              <button type="button" class="btn btn-primary">Men's</button>
            </div>
          </a>
        </div>
      </div>
    </section>

    <section class="bg-secondary py-4">
      <div class="container">
        <div class="row m-0">
          <div class="col-4">
            <picture>
              <source media="(min-width: 768px)" sizes="100vw" srcset="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" />
              <source sizes="100vw" srcset="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" />
              <img alt="Blog Post - Planting Trees with the Queen's Green Canopy " src="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" class="w-100"/>
            </picture>
          </div>
          <div class="col-8 d-flex align-items-center">
            <div>
              <h4>BLOG</h4>
              <h2>PLANTING TREES WITH THE QUEEN'S GREEN CANOPY</h2>
              <p>
                As part of The Regatta Group’s wider sustainability programme, Craghoppers, along with Regatta and Dare2b, is a platinum supporter of The Queen’s Green Canopy (QGC). This is a unique tree planting initiative, created in celebration of Her Majesty’s Platinum Jubilee in June this year, encouraging everyone all over the country to #PlantaTreefortheJubilee.
              </p>
              <a href="/community/busy-planting-trees-for-the-queens-jubilee/">Find Out More &gt;</a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from "@/components/homepage/carousel.vue";

export default {
  name: "Home",
  components: {
    Carousel,
  },
};
</script>
