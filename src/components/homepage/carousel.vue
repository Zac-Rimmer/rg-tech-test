<template>
  <div class="carousel">
    <div id="regattaCarousel" class="carousel slide" data-ride="carousel">
	  <div class="carousel-inner">
		<div class="carousel-item active">
			<picture>
				<source srcset="../../assets/images/banners/banner-1-mobile.jpeg" media="(max-width: 768px)" />
				<img src="../../assets/images/banners/banner-1.jpeg" alt="First slide" class="d-block w-100" />
			</picture>
		</div>
		<a href="/regatta-group" class="carousel-item">
		    <picture>
				<source srcset="../../assets/images/banners/banner-2-mobile.jpeg" media="(max-width: 768px)" />
				<img src="../../assets/images/banners/banner-2.jpeg" alt="Second slide" class="d-block w-100" />
			</picture>
            <div class="position-absolute start-0 end-0 bottom-0 text-center mb-4">
              <button type="button" class="btn btn-primary">Regatta Group</button>
            </div>
		</a>
		<div class="carousel-item">
		    <picture>
				<source srcset="../../assets/images/banners/banner-3-mobile.jpeg" media="(max-width: 768px)" />
				<img src="../../assets/images/banners/banner-3.jpeg" alt="Third slide" class="d-block w-100" />
			</picture>
		</div>
	  </div>
	</div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  props: {},
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