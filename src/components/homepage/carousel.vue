<template>
  <div class="carousel">
    <div class="carousel-inner">
      <transition-group
      class='carousel'
      tag="div">
        <div class="carousel-item" v-for="(slide,index) in slides" :key="slide.id">
            <div v-if="slide.id == 0">
              <picture>
                <source :srcset=slide.image_mobile media="(max-width: 767px)" />
                <img :src=slide.image alt="Main banner" :id="index" class="w-100" />
              </picture>
            </div> 
            <div v-if="slide.id == 1">
                <a href="/regatta-group">
                <picture>
                  <source :srcset=slide.image_mobile media="(max-width: 767px)" />
                  <img :src=slide.image alt="Main banner" :id="index" class="w-100" />
                </picture>
                <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
                  <button type="button" class="btn btn-primary">Regatta Group</button>
                </div>
                 </a>
            </div>
            <div v-if="slide.id == 2">
              <picture>
                <source :srcset=slide.image_mobile media="(max-width: 767px)" />
                <img :src=slide.image alt="Main banner" :id="index" class="w-100" />
              </picture>
            </div> 
        </div>
      </transition-group>
      <div class='carousel-controls'>
        <button class='carousel-controls__button arrow left' @click="previous"></button>
        <button class='carousel-controls__button arrow right' @click="next"></button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  props: {},
  data () {
    return {
      slides: [
        {
          id:0,
          image:require(`../../assets/images/banners/banner-1.jpeg`),
          image_mobile:require(`../../assets/images/banners/banner-1-mobile.jpeg`)
        },
        {
          id:1,
          image:require(`../../assets/images/banners/banner-2.jpeg`),
          image_mobile:require(`../../assets/images/banners/banner-2-mobile.jpeg`)
        },
        {
          id:2,
          image:require(`../../assets/images/banners/banner-3.jpeg`),
          image_mobile:require(`../../assets/images/banners/banner-3-mobile.jpeg`)
        }
    ],
    }
  },
  methods: {
    next () {
      const first = this.slides.shift()
      this.slides = this.slides.concat(first)
    },
    previous () {
      const last = this.slides.pop()
      this.slides = [last].concat(this.slides)
    }
  }
};
</script>

<style scoped lang="scss">
.arrow {
  border: solid black;
  border-width: 0 3px 3px 0;
  display: inline-block;
  padding: 3px;
  font-size:0;
}

.right {
  transform: rotate(-45deg);
  -webkit-transform: rotate(-45deg);
}

.left {
  transform: rotate(135deg);
  -webkit-transform: rotate(135deg);
  margin-right: 10px;
}

.carousel-item{
  display: block;
}

.carousel-inner{
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align:center;
}

img{
  width:100%;
}

.container .btn {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: #555;
  color: white;
  font-size: 16px;
  padding: 12px 24px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
}

.container .btn:hover {
  background-color: black;
}

</style>
