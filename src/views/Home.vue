<template>
  <div class="home">
    <Carousel />

    <section class="container my-4">
      <div class="row m-0">
        <div class="position-relative col-6">
          <picture>
              <source srcset="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C1-Mobile.jpg" media="(max-width: 768px)" />
              <img src="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C1-Desktop.jpg" alt="Shop Women's" class="w-100" />
           </picture>
           <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
              <button type="button" class="btn btn-primary" id="modal-btn" @click="popUp">Women's</button>
              <div class="modal">
                <div class="modal-content">
                  <span class="close-btn">&times;</span>
                  <p>This is the text inside the modal</p>
                </div>
              </div>
            </div>
        </div>
        <div class="position-relative col-6">
          <a href="/ie/outlet/mens/">
          <picture>
            <source srcset="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C2-Mobile.jpg" media="(max-width: 768px)" />
            <img src="https://cdn.regatta.com/images/uk/AW21/homepage/10-02-22/C2-Desktop.jpg" alt="Shop Men's" class="w-100" />
          </picture>
          <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
            <button type="button" class="btn btn-primary">Men's</button>
          </div>
          </a>
        </div>
      </div>
    </section>

    <section id="blog" class="py-4 col-12">
      <div class="row">
        <div class="col-lg-1 col-md-1 col-sm-2"></div>
        <div class="col-lg-3 col-md-5 col-sm-2"><img src="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" alt="Blog" id="blog-img" /></div>
        <div class="col-lg-6 col-md-6 col-sm-8">
           <h5 class="mt20 mb10">BLOG</h5>
           <h3 class="mt20 mb10">PLANTING TREES WITH THE QUEEN'S GREEN CANOPY</h3>

            <p>As part of The Regatta Group's wider sustainability programme, Craghoppers, along with Regatta 
            and Dare2b, is a platinum supporter of The Queen's Green Canopy (QGC). This is a unique tree 
            planting initiative, created in celebration of Her Majesty's Platinum Jubilee
            in June this year, encouraging everyone all over the country to #PlantaTreefortheJubilee.
            </p>
            <a href="/ie/outlet/womens/">Find Out More ></a>
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
  methods:{
    popUp(){
      let modalBtn = document.getElementById("modal-btn")
      let modal = document.querySelector(".modal")
      let closeBtn = document.querySelector(".close-btn")
      modalBtn.onclick = function(){
        modal.style.display = "block"
      }
      closeBtn.onclick = function(){
        modal.style.display = "none"
      }
      window.onclick = function(e){
        if(e.target == modal){
          modal.style.display = "none"
        }
      }
    }
  },
};
</script>
<style scoped lang="scss">

  #blog,#usp {
    background-color: #ddd;
  }
  #blog-img{
    height:auto;
    max-width:310px;
    vertical-align: middle;
  }
  .modal {
    display: none;
    position: fixed; 
    padding-top: 50px;
    left: 0; 
    top: 0;
    width: 100%;
    height: 100%; 
    background-color: rgb(0, 0, 0);
    background-color: rgba(0, 0, 0, 0.5);
  }
  .modal-content {
    position: relative; 
    background-color: white;
    padding: 20px; 
    margin: auto; 
    width: 75%;
  }
  .close-btn {
    float: right; 
    color: lightgray; 
    font-size: 24px;  
    font-weight: bold;
  }
  .close-btn:hover {
    color: darkgray;
  }
</style>