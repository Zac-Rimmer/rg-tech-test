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
	  
	<Blog />
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from "@/components/homepage/carousel.vue";
import Blog from "@/components/homepage/blog.vue";

export default {
  name: "Home",
  components: {
    Carousel,
	Blog,
  },
};
</script>

<style scoped lang="scss">
	.btn.btn-primary {
		border: 0;
		background-color: #000000;
		color: #ffffff;
		&:hover {
			background-color: #ffffff;
			color: #000000;
		}
	}
</style>